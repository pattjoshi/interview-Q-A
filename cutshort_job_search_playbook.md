# Cutshort Job Search Playbook — Om Prakash Pattjoshi

GenAI Engineer · 3 years · Python, FastAPI, LangChain, LangGraph, RAG, React.js, AWS
Last updated: November 1, 2026 (all links tested in the browser)

---

## 1. The main trick

Cutshort's best filter is **"Hiring activity on job"**. It shows jobs where the **recruiter was active recently**, not just when the job was posted.

Add `hiringActivityOnJob=1-days` to the link and you only see jobs where someone is reading applications **today**. Those recruiters reply faster.

---

## 2. How to use this file

1. Bookmark the links in section 4, one bookmarks folder for Cutshort.
2. Morning and evening: open the **Last 24 hours** links and apply to every good fit.
3. Once a day: open the **Last 3 days** links to catch anything you missed.
4. Once a week: open a link **without** `matchesfor=` to find jobs the profile matcher missed.
5. Skip any job that says *"The recruiter has not been active on this job recently."*

---

## 3. URL cheat sheet

Base: `https://cutshort.io/profile/all-jobs?`  (join each part with `&`)

| Parameter | What it does | Values |
|---|---|---|
| `hiringActivityOnJob=` | Recruiter active within this time | `1-days` (24 hrs) · `3-days` · `7-days` · `1-weeks` |
| `matchesfor=` | Only jobs matching your profile | `686d5e893771acfef1893691` (your code). Remove it to see **all** jobs |
| `remoteType=` | Workplace | `remote_only` · `remote_okay` (remote or office) · `remote_not_okay` (office only) |
| `locations=` | Cities | Join cities with a **dash `-`**, not a comma: `Bengaluru+%28Bangalore%29-Pune` |
| `minexp=` / `maxexp=` | Experience the job asks for | `minexp=2&maxexp=5` |
| `roletype=` | Job type | `full_time` · `internship` |
| `minsal=` + `salaryCurrency=` | Minimum salary, in rupees | `minsal=800000&salaryCurrency=INR` = ₹8 LPA |

Notes:
- `%28` = `(`, `%29` = `)`, `+` = space. Bengaluru must be written exactly `Bengaluru+%28Bangalore%29`.
- A comma between cities gives **zero results**. Always use `-`.
- `matchesfor=…` is your personal profile code. **Remove it before sharing a link publicly.**

---

## 4. Ready-to-use links

### Matched to your profile (best for daily applying)

| Search | Last 24 hours | Last 3 days |
|---|---|---|
| Your 4 cities (Bengaluru, Pune, Hyderabad, Noida) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29-Pune-Hyderabad-Noida&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29-Pune-Hyderabad-Noida&minexp=2&maxexp=5) |
| Remote only | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&remoteType=remote_only&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&remoteType=remote_only&minexp=2&maxexp=5) |
| Bengaluru | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29&minexp=2&maxexp=5) |
| Pune | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&locations=Pune&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&locations=Pune&minexp=2&maxexp=5) |
| Hyderabad | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&locations=Hyderabad&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&locations=Hyderabad&minexp=2&maxexp=5) |
| All locations, ₹10 LPA+ | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=1-days&roletype=full_time&minexp=2&maxexp=5&minsal=1000000&salaryCurrency=INR) | [Open](https://cutshort.io/profile/all-jobs?matchesfor=686d5e893771acfef1893691&hiringActivityOnJob=3-days&roletype=full_time&minexp=2&maxexp=5&minsal=1000000&salaryCurrency=INR) |

### All of Cutshort (no profile filter, safe to share)

| Search | Last 24 hours | Last 3 days |
|---|---|---|
| Remote only | [Open](https://cutshort.io/profile/all-jobs?hiringActivityOnJob=1-days&roletype=full_time&remoteType=remote_only&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?hiringActivityOnJob=3-days&roletype=full_time&remoteType=remote_only&minexp=2&maxexp=5) |
| Your 4 cities | [Open](https://cutshort.io/profile/all-jobs?hiringActivityOnJob=1-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29-Pune-Hyderabad-Noida&minexp=2&maxexp=5) | [Open](https://cutshort.io/profile/all-jobs?hiringActivityOnJob=3-days&roletype=full_time&locations=Bengaluru+%28Bangalore%29-Pune-Hyderabad-Noida&minexp=2&maxexp=5) |

---

## 5. Jobs with recruiters active in the past 24 hours

Snapshot from November 1, 2026, 00:30 IST: profile-matched, full-time, 2–5 years, all locations. Cutshort showed 20 jobs; 15 loaded on the page. Ranked by how well they fit your GenAI / Python resume.

### Best fit — apply first

| # | Role | Company | Location | Exp | Salary | Link |
|---|---|---|---|---|---|---|
| 1 | Senior Fullstack Engineer | AI-powered tech company (via Cutshort Lightning) | Remote / Bengaluru | 3–6 yrs | Up to ₹39L | [Apply](https://cutshort.io/job/Senior-Fullstack-Engineer-Bengaluru-Bangalore-Cutshort-Lightning-encbzjFp) |
| 2 | Mid-Level Backend, Data & ML Developer | Quixta | Remote only | 3–7 yrs | ₹15L–19L | [Apply](https://cutshort.io/job/Mid-Level-Backend-Data-ML-Developer-Quixta-g0bnhxsk) |
| 3 | Sr Software Engineer (Backend, Python) | WordPress cloud platform (via Cutshort Lightning) | Bengaluru | 3–5 yrs | Up to ₹28L | [Apply](https://cutshort.io/job/Sr-Software-Engineer-Backend-Bengaluru-Bangalore-Cutshort-Lightning-hI7aAX0b) |
| 4 | Data Science Engineer | Talview | Bengaluru | 3–5 yrs | ₹15L–25L | [Apply](https://cutshort.io/job/Data-Science-Engineer-Bengaluru-Bangalore-Talview-rdyG0fTC) |
| 5 | Customer Solution Engineer – AI | MyOperator (VoiceTree) | Delhi NCR / Noida | 2–5 yrs | ₹8L–12L | [Apply](https://cutshort.io/job/Customer-Solution-Engineer-AI-Delhi-Gurugram-Noida-Ghaziabad-Faridabad-MyOperator-VoiceTree-Technologies-BJ9adkhg) |
| 6 | Backend Developer II (Python / Go) | HyrHub (agency) | Bengaluru | 2–4 yrs | ₹8L–12L | [Apply](https://cutshort.io/job/Backend-Developer-II-Python-Go-Bengaluru-Bangalore-HyrHub-A4tZKyjJ) |
| 7 | Full Stack Developer | Metron Security | Pune / Bengaluru | 3–6 yrs | ₹6L–12L | [Apply](https://cutshort.io/job/Full-Stack-Developer-Pune-Bengaluru-Bangalore-Metron-Security-Private-Limited-YcfkP61e) |
| 8 | Full Stack Web Developer (React / Node) | JKYog | Remote only | 3–7 yrs | ₹15L–30L | [Apply](https://cutshort.io/job/Full-Stack-Web-Developer-JavaScript-React-Node-js-JKYog-fNfNldjD) |

### Maybe — read the job first

| # | Role | Company | Location | Exp | Salary | Why maybe | Link |
|---|---|---|---|---|---|---|---|
| 9 | Backend Engineer | GeoIQ | Bengaluru | 2–4 yrs | Not shown | General backend | [Open](https://cutshort.io/job/Backend-Engineer-Bengaluru-Bangalore-GeoIQ-63gmA9Gf) |
| 10 | Computer Vision Engineer | Inferigence Quotient | Bengaluru | 2–3 yrs | ₹8L–15L | Vision, not LLM | [Open](https://cutshort.io/job/Computer-Vision-Engineer-Bengaluru-Bangalore-Inferigence-Quotient-jjcN4pX1) |
| 11 | AI & Python Course Instructor | Neuronetwrk AI ED | Pune | 3–8 yrs | ₹10L–15L | Teaching role | [Open](https://cutshort.io/job/AI-Python-Course-Instructor-Pune-Neuronetwrk-AI-ED-hCPQ2FFf) |
| 12 | Technical Product Catalyst – Fintech | Cambridge Wealth | Pune | 2–6 yrs | ₹8L–13L | Product + Django | [Open](https://cutshort.io/job/Technical-Product-Catalyst-Fintech-Pune-Cambridge-Wealth-Baker-Street-Fintech--cBesqLRC) |
| 13 | Full-Stack Developer (React Native + Python) | JARK Technologies | Remote only | 2–4 yrs | ₹5L–8L | Low pay | [Open](https://cutshort.io/job/Full-Stack-Developer-React-Native-and-Python-JARK-Technologies-gSlcYaAu) |
| 14 | Full-Stack Developer (On-site) | UPRIGHT LLC | Hyderabad | 3–6 yrs | ₹4L–6L | Below your current pay | [Open](https://cutshort.io/job/Full-Stack-Developer-3-5-Years-On-Site-Hyderabad-Hyderabad-UPRIGHT-LLC-8f3LirRm) |
| 15 | Software Craftsperson (Ruby on Rails) | Incubyte | Remote only | 2–5 yrs | Not shown | Ruby, not your stack | [Open](https://cutshort.io/job/Software-Craftsperson-ROR-II-Incubyte-PKqRJ6q6) |

These change every day. Use the "Last 24 hours" links in section 4 for the latest list.

---

## 6. Apply checklist (per job)

- [ ] Recruiter active in the last 24 hours (no "not active recently" warning)
- [ ] Required experience fits 2–5 years
- [ ] Stack matches at least 3 of: Python, FastAPI, LangChain/LangGraph, RAG, vector DB, React, AWS
- [ ] Add a 2-line note with one metric:
  - RAG course assistant with citations for an LMS
  - ~20% fewer out-of-scope / hallucinated answers
  - ~20% lower latency, ~15% lower token cost via Langfuse
- [ ] Reply to any recruiter message within a day

### Short note when applying (edit per job)

> Hi [Name], I'm a GenAI Engineer with 3 years of experience building RAG pipelines and LangGraph agents in production with Python and FastAPI. In my last role I cut hallucinated answers by ~20% and token cost by ~15%. I can join immediately and would love to talk about the [Role] role.

---

## 7. Daily tracker

| Date | Company | Role | Link | Recruiter active? | Status | Follow-up |
|---|---|---|---|---|---|---|
| | | | | | | |
