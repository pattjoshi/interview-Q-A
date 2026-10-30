# LinkedIn Job Search Playbook — Om Prakash Pattjoshi

GenAI Engineer · 3 years · Python, FastAPI, LangChain, LangGraph, RAG, React.js, AWS
Last updated: October 2026

---

## 1. How to use this file

1. Bookmark the links below in your browser, one folder per role.
2. Morning: open the **Last 24 hours** links and apply to the best fits.
3. 2–3 times during the day: open the **Last 1 hour** links and apply fast to anything new.
4. On each job, check the applicant count. Prioritise "Be an early applicant" and under 25 applicants.

All links use: experience = Associate + Mid-Senior (`f_E=3%2C4`), newest first (`sortBy=DD`).

---

## 2. URL cheat sheet

Base: `https://www.linkedin.com/jobs/search/?`

| Parameter | What it does | Values |
|---|---|---|
| `keywords=` | Role or Boolean search | `GenAI%20Engineer` (`%20` = space) |
| `location=` | Place name | `India`, `Bengaluru, Karnataka, India`, `Worldwide` |
| `geoId=` | Exact LinkedIn location ID | India `102713980`, Worldwide `92000000`. City links use the city name only, so LinkedIn matches it for you. |
| `f_TPR=` | Time since posted (seconds) | `r3600` 1 hr · `r7200` 2 hr · `r86400` 24 hr · `r604800` week |
| `f_WT=` | Workplace | `1` on-site · `2` remote · `3` hybrid · `2%2C3` remote + hybrid |
| `f_E=` | Experience level | `2` entry · `3` associate · `4` mid-senior |
| `f_JT=` | Job type | `F` full-time · `C` contract |
| `f_AL=true` | Easy Apply only | — |
| `sortBy=DD` | Newest first | `R` = most relevant |
| `start=` | Next page (25 per page) | `25`, `50`, `75` |

Notes:
- `%2C` = comma, used to combine values.
- `r3600` is not in LinkedIn's menu; it is a URL-only trick. If results look old, open the "Date posted" filter once in the UI and re-apply.
- If a city link opens the wrong place, pick the city in LinkedIn's location box and copy the `geoId` it adds to the URL.
- Getting too few results at 3 years? Add entry level: change `f_E=3%2C4` to `f_E=2%2C3%2C4`. Many Indian companies tag 2–4 year roles as entry level.
- Bookmark tip: put the 1-hour links in one bookmarks folder, then right-click the folder → "Open all" to check every search in one go.

---

## 3. Ready-to-use links

### GenAI Engineer

| Location | Last 1 hour | Last 24 hours |
|---|---|---|
| All of India | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Remote (India) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |
| Bengaluru | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Pune | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Hyderabad | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Worldwide remote | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |

### LLM / AI Engineer

| Location | Last 1 hour | Last 24 hours |
|---|---|---|
| All of India | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Remote (India) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |
| Bengaluru | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Pune | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Hyderabad | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Worldwide remote | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |

### AI Engineer

| Location | Last 1 hour | Last 24 hours |
|---|---|---|
| All of India | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Remote (India) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |
| Bengaluru | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Pune | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Hyderabad | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Worldwide remote | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |

### Python / FastAPI Developer

| Location | Last 1 hour | Last 24 hours |
|---|---|---|
| All of India | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Remote (India) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |
| Bengaluru | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Pune | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Hyderabad | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Worldwide remote | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Worldwide&geoId=92000000&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20FastAPI%20Developer&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |

### Full Stack AI Developer

| Location | Last 1 hour | Last 24 hours |
|---|---|---|
| All of India | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Remote (India) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=India&geoId=102713980&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |
| Bengaluru | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Bengaluru%2C%20Karnataka%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Pune | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Pune%2C%20Maharashtra%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Hyderabad | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r3600&f_E=3%2C4&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Hyderabad%2C%20Telangana%2C%20India&f_TPR=r86400&f_E=3%2C4&sortBy=DD) |
| Worldwide remote | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Worldwide&geoId=92000000&f_TPR=r3600&f_E=3%2C4&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20AI%20Developer&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD) |

### Power search (Boolean, all your skills in one link)

Keyword: `("GenAI" OR "Generative AI" OR "LLM") AND (Python OR LangChain OR RAG)`

- All of India, last 24 hours: [Open](https://www.linkedin.com/jobs/search/?keywords=%28%22GenAI%22%20OR%20%22Generative%20AI%22%20OR%20%22LLM%22%29%20AND%20%28Python%20OR%20LangChain%20OR%20RAG%29&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&sortBy=DD)
- Remote (India), last 24 hours: [Open](https://www.linkedin.com/jobs/search/?keywords=%28%22GenAI%22%20OR%20%22Generative%20AI%22%20OR%20%22LLM%22%29%20AND%20%28Python%20OR%20LangChain%20OR%20RAG%29&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD)
- Worldwide remote, last 24 hours: [Open](https://www.linkedin.com/jobs/search/?keywords=%28%22GenAI%22%20OR%20%22Generative%20AI%22%20OR%20%22LLM%22%29%20AND%20%28Python%20OR%20LangChain%20OR%20RAG%29&location=Worldwide&geoId=92000000&f_TPR=r86400&f_E=3%2C4&f_WT=2&sortBy=DD)
- All of India, last 24 hours, Easy Apply only: [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&geoId=102713980&f_TPR=r86400&f_E=3%2C4&f_AL=true&sortBy=DD)

---

## 4. Keywords that match your resume

Use these in `keywords=` or in the Boolean search:

- Titles: GenAI Engineer, Generative AI Engineer, LLM Engineer, AI Engineer, Applied AI Engineer, AI/ML Engineer, Python Developer (AI), Full Stack AI Developer
- Skills recruiters search: RAG, LangChain, LangGraph, Agentic AI, AI Agents, OpenAI, FastAPI, Vector Database, Pinecone, pgvector, LLMOps, Prompt Engineering, AWS Bedrock

Boolean tips: use `AND`, `OR`, `NOT` in capitals; put phrases in quotes; group with brackets.
Example: `("LLM Engineer" OR "GenAI Engineer") AND RAG NOT intern`

---

## 5. Apply checklist (per job)

- [ ] Posted under 24 hours, ideally under 1 hour
- [ ] Required experience fits 2–5 years
- [ ] Stack matches at least 3 of: Python, FastAPI, LangChain/LangGraph, RAG, vector DB, React, AWS
- [ ] Resume headline matches the job title (GenAI / LLM / AI Engineer)
- [ ] Mention one metric in the note or cover letter:
  - RAG course assistant with citations for an LMS
  - ~20% fewer out-of-scope / hallucinated answers
  - ~20% lower latency, ~15% lower token cost via Langfuse
- [ ] After applying: message the recruiter or hiring manager within 24 hours

### Short recruiter note (edit per job)

> Hi [Name], I just applied for the [Role] role at [Company]. I'm a GenAI Engineer with 3 years of experience building RAG pipelines and LangGraph agents in production with Python and FastAPI. I'd love to be considered. Thank you!

---

## 6. Daily tracker

| Date | Company | Role | Link | Applicants when applied | Status | Follow-up |
|---|---|---|---|---|---|---|
| | | | | | | |
