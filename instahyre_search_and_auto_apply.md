# Instahyre Search Tricks + Auto-Apply Script

For: Om Prakash Pattjoshi, GenAI Engineer, 3 years
Last updated: 1 Nov 2026

---

## 1. Search tricks (tested 31 Oct 2026)

Instahyre's public search page reads filters straight from the link, so you can bookmark any search.

Base: `https://www.instahyre.com/search-jobs/?`

| Parameter | What it does | Values |
|---|---|---|
| `skills=` | Skills or titles, matched with OR | `LangChain` · several: `LangChain,RAG,Generative%20AI` (`%20` = space) |
| `years=` | Your experience | `3` |
| `location=` | City or remote | `Bangalore`, `Pune`, `Hyderabad`, `Mumbai`, `Gurgaon`, `Work%20From%20Home` · several: `Work%20From%20Home,Bangalore` |
| `job_functions=` | Job category | `/api/v1/job_function/9` Data Science / ML · `/10` Backend · `/1` Full-Stack · `/8` DevOps / Cloud · several: comma-separated |
| `company_size=` | Company size | `1` small (startups) · `3` medium · `2` large |

Tested counts: LangChain at 3 years = 185 jobs. LangChain + RAG + Generative AI = 1,397. Same, startups only = 721.

Tips:
- Leave a parameter out to mean "all".
- Spell cities the way Instahyre does (Bangalore, not Bengaluru).
- Instahyre has **no "posted in last hour" filter** (menu or URL). Stay early by checking morning and evening.
- More skills = more jobs (it's OR). Add `job_functions` or `company_size` to narrow down.

### Ready links

| Search | Link |
|---|---|
| All your skills, all India | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,LLMs,LangChain,LangGraph,RAG,Agentic%20AI,FastAPI |
| All your skills, remote + Bangalore + Pune + Hyderabad | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,LLMs,LangChain,LangGraph,RAG,Agentic%20AI,FastAPI&location=Work%20From%20Home,Bangalore,Pune,Hyderabad |
| Startups only | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,LLMs,LangChain,LangGraph,RAG,Agentic%20AI,FastAPI&company_size=1 |
| Data Science / ML category only | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,LLMs,LangChain,LangGraph,RAG,Agentic%20AI,FastAPI&job_functions=/api/v1/job_function/9 |
| GenAI / LLM, remote | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,LLMs,LangChain,RAG&location=Work%20From%20Home |
| Agentic AI, Pune | https://www.instahyre.com/search-jobs/?years=3&skills=Agentic%20AI,LangGraph&location=Pune |
| Python FastAPI, Bangalore | https://www.instahyre.com/search-jobs/?years=3&skills=FastAPI&location=Bangalore |
| Full Stack AI, remote | https://www.instahyre.com/search-jobs/?years=3&skills=Generative%20AI,React.js&job_functions=/api/v1/job_function/1&location=Work%20From%20Home |

---

## 2. Auto-apply script (paste in browser console)

### Read this first
- **Account risk:** bulk auto-applying may break Instahyre's terms of use and can get your account flagged or limited. Keep `MAX_APPLY` small (10–20 a day) and the delays as they are.
- **Quality beats quantity:** recruiters see every application. Applying to badly-matched jobs can hurt your reply rate.
- **Partly untested:** the job cards' **"View job »"** button (`button.btn-interested`) was confirmed on 31 Oct 2026. The **Apply** button inside the job popup was not inspected, so the script finds it by its text ("Apply" / "I'm interested"). Run it in **dry-run mode first**.
- Use it only on your own account, signed in, in your own browser.

### How to run
1. Sign in to Instahyre in Chrome.
2. Open one of the search links above (desktop width, so job cards are visible).
3. Press `F12` (or `Ctrl+Shift+J`) and open the **Console** tab.
4. If Chrome blocks pasting, type `allow pasting` and press Enter.
5. Paste the script and press Enter.
6. First run: keep `DRY_RUN = true`. It only lists what it *would* apply to.
7. If the list looks right, set `DRY_RUN = false` and run again.
8. To stop at any time, type `window.__stopApply = true` and press Enter, or reload the page.

### Script

```javascript
(async () => {
  // ===== SETTINGS =====
  const DRY_RUN = true;          // true = only log, no applying. Set false to apply.
  const MAX_APPLY = 15;          // max applications per run
  const MIN_DELAY = 6000;        // ms, minimum wait between jobs
  const MAX_DELAY = 12000;       // ms, maximum wait between jobs
  // Only apply if job text contains at least one of these (case-insensitive):
  const MUST_HAVE = ['genai', 'generative ai', 'llm', 'langchain', 'langgraph', 'rag', 'agentic', 'fastapi'];
  // Skip if job text contains any of these:
  const SKIP_IF = ['intern', 'senior manager', 'principal', 'director', '8+ years', '10+ years', 'java developer'];
  // ====================

  const sleep = (ms) => new Promise(r => setTimeout(r, ms));
  const rand = () => MIN_DELAY + Math.random() * (MAX_DELAY - MIN_DELAY);
  const visible = (el) => el && el.offsetParent !== null;
  const textOf = (el) => (el?.innerText || '').toLowerCase();

  // Finds a visible button/link whose text matches the pattern
  const findButton = (pattern, root = document) =>
    [...root.querySelectorAll('button, a')].find(b => visible(b) && pattern.test(b.innerText.trim()));

  window.__stopApply = false;
  let applied = 0, skipped = 0, seen = new Set();
  console.log(`%cInstahyre auto-apply started (DRY_RUN=${DRY_RUN})`, 'color:#0a0;font-weight:bold');

  while (applied < MAX_APPLY && !window.__stopApply) {
    // Job cards: each has a "View job »" button with class btn-interested
    const cards = [...document.querySelectorAll('button.btn-interested')]
      .filter(b => visible(b) && !seen.has(b));

    if (!cards.length) {
      // Try loading more results by scrolling, else stop
      window.scrollTo(0, document.body.scrollHeight);
      await sleep(3000);
      const more = [...document.querySelectorAll('button.btn-interested')].filter(b => visible(b) && !seen.has(b));
      if (!more.length) { console.log('No more jobs on this page.'); break; }
      continue;
    }

    const btn = cards[0];
    seen.add(btn);
    const card = btn.closest('[class*="employer"], [class*="opportunity"], li, .row') || btn.parentElement;
    const cardText = textOf(card);
    const title = (card?.querySelector('a, h2, h3, .employer-job-name')?.innerText || cardText.slice(0, 80)).trim();

    if (SKIP_IF.some(w => cardText.includes(w)) || !MUST_HAVE.some(w => cardText.includes(w))) {
      skipped++;
      console.log(`Skip: ${title}`);
      continue;
    }

    if (DRY_RUN) {
      applied++;
      console.log(`%c[DRY RUN] Would apply: ${title}`, 'color:#06c');
      continue;
    }

    // Open the job popup
    btn.scrollIntoView({ block: 'center' });
    btn.click();
    await sleep(2500);

    // Find the Apply / Interested button inside the popup (matched by text; not inspected in testing)
    const applyBtn = findButton(/^(apply|i'?m interested|interested)\b/i);
    if (applyBtn && !applyBtn.disabled) {
      applyBtn.click();
      applied++;
      console.log(`%cApplied (${applied}/${MAX_APPLY}): ${title}`, 'color:#0a0');
      await sleep(2000);
    } else {
      skipped++;
      console.log(`No Apply button found (maybe already applied): ${title}`);
    }

    // Close the popup if it is still open
    const closeBtn = document.querySelector('.modal.in .close, .modal.show .close, [aria-label="Close"]');
    if (visible(closeBtn)) closeBtn.click();
    else document.dispatchEvent(new KeyboardEvent('keydown', { key: 'Escape', bubbles: true }));

    await sleep(rand());
  }

  console.log(`%cDone. ${DRY_RUN ? 'Would apply' : 'Applied'}: ${applied}, skipped: ${skipped}`, 'color:#0a0;font-weight:bold');
})();
```

### If the script says "No Apply button found" for every job
Instahyre may label the button differently. Open one job by hand, right-click its Apply button → **Inspect**, and note the text or class. Then change this line to match:

```javascript
const applyBtn = findButton(/^(apply|i'?m interested|interested)\b/i);
// e.g. by class instead:
// const applyBtn = document.querySelector('.modal.in button.btn-apply');
```

---

## 3. Daily routine
1. Morning: open 3–4 bookmarked links, run the script in dry-run, check the list, then apply.
2. Evening: open the links again and apply by hand to the best new jobs.
3. Reply to recruiter messages in the Inbox the same day.
4. For your top 5 jobs, find the recruiter on LinkedIn and send a 2-line note with one metric (~20% lower latency, ~20% fewer hallucinated answers).

## 4. Tracker

| Date | Company | Role | Link | Status | Follow-up |
|---|---|---|---|---|---|
| | | | | | |
