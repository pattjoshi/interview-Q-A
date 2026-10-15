# Job Search URL Guide – Naukri & LinkedIn

**For:** Om Prakash Pattjoshi · GenAI Engineer · 3 yrs · Hyderabad
**Goal:** Open the right job list in one click, without setting filters by hand every time.

---

## 1. How a Naukri search URL works

```
https://www.naukri.com/<keyword-slug>-jobs[-in-<city>][-<page>]?k=<keyword>&l=<city>&experience=<years>&jobAge=<days>&wfhType=<mode>
```

| Part | What it does | Values | Checked? |
|---|---|---|---|
| `<keyword-slug>-jobs` | Page path. Use the keyword with spaces replaced by `-` | `genai-jobs`, `python-developer-jobs` | ✅ |
| `-in-<city>` | Optional city in the path (good to keep with `l=`) | `-in-hyderabad` | ✅ |
| `-<page>` | Page number (20 jobs per page). Page 1 has no number | `genai-jobs-2`, `genai-jobs-3` | ✅ |
| `k=` | **Keyword(s)**. Space = `%20`, several keywords = comma `%2C` | `k=genai`, `k=python%20developer` | ✅ |
| `l=` | **Location**. Several cities = comma | `l=hyderabad`, `l=hyderabad%2Cbengaluru` | ✅ |
| `experience=` | **Your years of experience**. Shows jobs whose range includes this number | `experience=3` | ✅ |
| `jobAge=` | **Freshness**: posted within last N days | `1`, `3`, `7`, `15`, `30` | ✅ |
| `wfhType=` | **Work mode** | `0` = Office, `2` = Remote, `3` = Hybrid | ✅ (3 tested, 2 accepted) |

> **Important rule:** The path slug and `k=` must match. If you change `k=` but keep an old slug, Naukri may ignore your filters (this happened during testing).

**Sorting by date / salary filter / company type:** These did not stay in the URL when tested. Set them on the page instead: **Sort by → Date** (top-right), **Salary** (left filter panel).

---

## 2. LinkedIn search URL (for later)

```
https://www.linkedin.com/jobs/search/?keywords=<keyword>&location=<place>&f_TPR=<time>&f_AL=true&f_WT=<mode>&f_E=<level>&sortBy=DD
```

| Parameter | Meaning | Values |
|---|---|---|
| `keywords=` | Keyword | `GenAI%20Engineer` |
| `location=` | Place | `India`, `Hyderabad` |
| `f_TPR=` | Posted within | `r3600` = 1 hour, `r86400` = 24 hours, `r604800` = 1 week |
| `f_AL=true` | **Easy Apply only** | – |
| `f_WT=` | Work mode | `1` = On-site, `2` = Remote, `3` = Hybrid (comma for several: `2%2C3`) |
| `f_E=` | Experience level | `2` = Entry, `3` = Associate, `4` = Mid-Senior (for you: `2%2C3`) |
| `sortBy=DD` | Newest first | `R` = most relevant |

> LinkedIn did not respond to browser automation in this session, so these were not tested live. They are LinkedIn's standard search parameters.

---

## 3. Your keyword list (based on your profile)

**GenAI / AI (best fit, apply first)**
`genai` · `generative ai` · `llm` · `ai engineer` · `langchain` · `agentic ai` · `rag` · `ai agents`

**Python / Backend**
`python developer` · `fastapi` · `python backend developer`

**Full stack**
`full stack developer` · `react developer` · `next.js`

## 4. Locations and work modes (your priority order)

| Priority | Naukri | LinkedIn |
|---|---|---|
| 1. Remote | `wfhType=2` (no `l=`) | `location=India&f_WT=2` |
| 2. Hyderabad | `-in-hyderabad` + `l=hyderabad` | `location=Hyderabad` |
| 3. Hybrid | `wfhType=3` | `f_WT=3` |
| 4. All India | no `l=`, no `wfhType` | `location=India` |

## 5. All combinations

**Total = 14 keywords × 4 location modes × 5 freshness options = 280 Naukri searches** (plus the same again for LinkedIn).
You do **not** need all of them. Daily, use **freshness = 1 day** → 14 × 4 = **56 searches**, and the top 4 keywords cover most jobs.

### 5a. Ready-to-click Naukri links (last 24 h, 3 yrs exp)

| Keyword | Remote | Hyderabad | Hybrid | All India |
|---|---|---|---|---|
| GenAI | [Open](https://www.naukri.com/genai-jobs?k=genai&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/genai-jobs-in-hyderabad?k=genai&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/genai-jobs?k=genai&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/genai-jobs?k=genai&experience=3&jobAge=1) |
| Generative AI | [Open](https://www.naukri.com/generative-ai-jobs?k=generative%20ai&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/generative-ai-jobs-in-hyderabad?k=generative%20ai&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/generative-ai-jobs?k=generative%20ai&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/generative-ai-jobs?k=generative%20ai&experience=3&jobAge=1) |
| LLM | [Open](https://www.naukri.com/llm-jobs?k=llm&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/llm-jobs-in-hyderabad?k=llm&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/llm-jobs?k=llm&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/llm-jobs?k=llm&experience=3&jobAge=1) |
| AI Engineer | [Open](https://www.naukri.com/ai-engineer-jobs?k=ai%20engineer&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/ai-engineer-jobs-in-hyderabad?k=ai%20engineer&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/ai-engineer-jobs?k=ai%20engineer&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/ai-engineer-jobs?k=ai%20engineer&experience=3&jobAge=1) |
| LangChain | [Open](https://www.naukri.com/langchain-jobs?k=langchain&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/langchain-jobs-in-hyderabad?k=langchain&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/langchain-jobs?k=langchain&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/langchain-jobs?k=langchain&experience=3&jobAge=1) |
| Agentic AI | [Open](https://www.naukri.com/agentic-ai-jobs?k=agentic%20ai&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/agentic-ai-jobs-in-hyderabad?k=agentic%20ai&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/agentic-ai-jobs?k=agentic%20ai&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/agentic-ai-jobs?k=agentic%20ai&experience=3&jobAge=1) |
| RAG | [Open](https://www.naukri.com/rag-jobs?k=rag&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/rag-jobs-in-hyderabad?k=rag&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/rag-jobs?k=rag&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/rag-jobs?k=rag&experience=3&jobAge=1) |
| AI Agents | [Open](https://www.naukri.com/ai-agents-jobs?k=ai%20agents&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/ai-agents-jobs-in-hyderabad?k=ai%20agents&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/ai-agents-jobs?k=ai%20agents&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/ai-agents-jobs?k=ai%20agents&experience=3&jobAge=1) |
| Python Developer | [Open](https://www.naukri.com/python-developer-jobs?k=python%20developer&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/python-developer-jobs-in-hyderabad?k=python%20developer&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/python-developer-jobs?k=python%20developer&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/python-developer-jobs?k=python%20developer&experience=3&jobAge=1) |
| FastAPI | [Open](https://www.naukri.com/fastapi-jobs?k=fastapi&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/fastapi-jobs-in-hyderabad?k=fastapi&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/fastapi-jobs?k=fastapi&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/fastapi-jobs?k=fastapi&experience=3&jobAge=1) |
| Python Backend | [Open](https://www.naukri.com/python-backend-developer-jobs?k=python%20backend%20developer&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/python-backend-developer-jobs-in-hyderabad?k=python%20backend%20developer&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/python-backend-developer-jobs?k=python%20backend%20developer&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/python-backend-developer-jobs?k=python%20backend%20developer&experience=3&jobAge=1) |
| Full Stack Developer | [Open](https://www.naukri.com/full-stack-developer-jobs?k=full%20stack%20developer&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/full-stack-developer-jobs-in-hyderabad?k=full%20stack%20developer&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/full-stack-developer-jobs?k=full%20stack%20developer&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/full-stack-developer-jobs?k=full%20stack%20developer&experience=3&jobAge=1) |
| React Developer | [Open](https://www.naukri.com/react-developer-jobs?k=react%20developer&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/react-developer-jobs-in-hyderabad?k=react%20developer&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/react-developer-jobs?k=react%20developer&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/react-developer-jobs?k=react%20developer&experience=3&jobAge=1) |
| Next.js | [Open](https://www.naukri.com/next-js-jobs?k=next.js&experience=3&jobAge=1&wfhType=2) | [Open](https://www.naukri.com/next-js-jobs-in-hyderabad?k=next.js&l=hyderabad&experience=3&jobAge=1) | [Open](https://www.naukri.com/next-js-jobs?k=next.js&experience=3&jobAge=1&wfhType=3) | [Open](https://www.naukri.com/next-js-jobs?k=next.js&experience=3&jobAge=1) |

**To change freshness:** replace `jobAge=1` with `3`, `7`, `15` or `30`.
**To see page 2:** add `-2` after `-jobs` (e.g. `genai-jobs-2?...`).

### 5b. Ready-to-click LinkedIn links (last 24 h, Easy Apply, newest first)

| Keyword | Remote | Hyderabad | All India |
|---|---|---|---|
| GenAI Engineer | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&f_TPR=r86400&f_AL=true&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=Hyderabad&f_TPR=r86400&f_AL=true&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=GenAI%20Engineer&location=India&f_TPR=r86400&f_AL=true&sortBy=DD) |
| AI Engineer | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&f_TPR=r86400&f_AL=true&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=Hyderabad&f_TPR=r86400&f_AL=true&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=AI%20Engineer&location=India&f_TPR=r86400&f_AL=true&sortBy=DD) |
| LLM Engineer | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&f_TPR=r86400&f_AL=true&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=Hyderabad&f_TPR=r86400&f_AL=true&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=LLM%20Engineer&location=India&f_TPR=r86400&f_AL=true&sortBy=DD) |
| Python Developer | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20Developer&location=India&f_TPR=r86400&f_AL=true&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20Developer&location=Hyderabad&f_TPR=r86400&f_AL=true&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Python%20Developer&location=India&f_TPR=r86400&f_AL=true&sortBy=DD) |
| Full Stack Developer | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20Developer&location=India&f_TPR=r86400&f_AL=true&f_WT=2&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20Developer&location=Hyderabad&f_TPR=r86400&f_AL=true&sortBy=DD) | [Open](https://www.linkedin.com/jobs/search/?keywords=Full%20Stack%20Developer&location=India&f_TPR=r86400&f_AL=true&sortBy=DD) |

---

## 6. Recommended daily routine (about 20 minutes)

1. **Morning (8–10 am):** new jobs have fewer applicants, so recruiters are more likely to see you.
2. Open the **Remote** column, then **Hyderabad**, then **All India**: GenAI → AI Engineer → LLM → Python → Full Stack.
3. Only click jobs showing **"Apply"** (not "Apply on company site" – those take longer; do them separately if the company is good).
4. **One application per company per day.** Some staffing firms post the same job in 8 cities, so applying to all of them wastes your daily limit.
5. **Naukri daily limit ≈ 50 applications.** After that you get "There was an error while processing your request". Stop and continue the next day.
6. **Skip:** Infosys, Deloitte, Accenture, Capgemini (your choice), and roles needing Java, .NET, PHP/Laravel, Oracle, Flutter or React Native. Also skip "training programs" that ask for money.

## 7. Standard answers for recruiter questions

| Question | Your answer |
|---|---|
| Total experience | 3 years |
| Python / GenAI / LLM / React / JavaScript experience | 3 years |
| AWS / Database experience | 2 years |
| Notice period | 15 days (available to join within 15 days) |
| Current CTC | 6.5 LPA |
| Expected CTC | 6.5 LPA (you chose this; consider 8–9 LPA for a normal hike) |
| Current location | Hyderabad |
| Willing to relocate / work from office / F2F interview | Yes |
| Current company / designation | Transcom / GenAI Engineer (**update this if you have left Transcom**) |
| Highest qualification | B.Tech, Computer Science and Engineering (2024) |
| Reason for job change | Looking for a more challenging GenAI engineering role with better growth |

## 8. Tips to get more recruiter calls

- **Update your Naukri profile every morning.** Even a small edit pushes you higher in recruiter searches.
- Fix the **employment gap**: your profile shows Transcom ended Jul 2026. Recruiters notice this, so add a current status or short note.
- **Message recruiters** after applying to good matches (Naukri "Recruiter" link or LinkedIn): 2–3 lines on your GenAI/RAG/LangGraph experience.
- Add your **LinkedIn URL** to your Naukri profile. Several forms ask for it, and jobs that require it get skipped without it.
