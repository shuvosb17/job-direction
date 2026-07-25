# v2.1 — Remote Fresher Only (Ruthlessly Cut)

**Goal:** Land a **first backend role** (remote preferred; local/intern/contract acceptable) in **8–10 months**, not become a staff engineer on paper.

**Budget:** 30 hrs/week  
**Rule:** If it doesn’t help you **apply, interview, or get a callback** by month 5, it’s cut or deferred.

---

## What Changed From v2

| v2 | v2.1 |
|----|------|
| 5 flagships + AI layer + full AWS course | **2 live flagships** + optional 3rd if interviewing |
| 24 modules, ~50 projects | **12 modules**, **8 projects** that matter |
| Apply month 5 after heavy build | **Apply month 4** with 1 live project |
| Capstone = fintech ledger + OTel + AI | **Deferred** until after first job or strong pipeline |
| Success = finish curriculum | Success = **applications + interviews + offer** |

---

## KEEP (Non-Negotiable)

### Modules / skills
- **M0** — Git, CLI, how the web works  
- **M1** — Go fundamentals  
- **M2** — Concurrency basics (goroutines, channels, context — not every pattern)  
- **M3** — Unit + 1 integration test  
- **M4** — REST API, middleware, status codes, validation  
- **M5** — Postgres, SQL, migrations, transactions  
- **M6** — JWT, bcrypt, RBAC basics, SQL injection prevention  
- **M9** — Docker + docker-compose  
- **M7 (lite)** — Deploy to one Linux VM or ECS (pick one path)  
- **M12 (lite)** — EC2 or ECS + RDS + S3 basics (not full AWS cert path)  
- **M23 (lite)** — Resume, LinkedIn, applications, mock interviews  
- **Instructor course (concept only)** — API dev, DB/ERD, JWT, security, pagination, CORS  

### Projects
1. **`jobtrackr`** — Flagship 1 (must be live, you use it for applications)  
2. **`vaultdrop` lite** — File upload + auth + S3 OR simplified second API (must be live)  
3. **Git workflow repo** — from M0  

### Job hunt (parallel from month 4)
- DSA: **5–8 hrs/week** (NeetCode Easy/Medium in Go)  
- Applications: **8–12/week** from month 4  
- Outreach: **5 personalized messages/week**  
- 1 **contract/intern** attempt every month from month 5  

---

## DELETE or DEFER (Post-First-Job)

| Cut from v2.1 | Why |
|---------------|-----|
| **`taka-flow` capstone** | Senior scope; delays applying 2–3 months |
| **`hookrelay`** | Build only if you have extra time while interviewing |
| **`pulsewatch`** | Nice demo, zero hire impact vs 20 more applications |
| **`askvault` RAG / full M17 AI** | Optional stretch; 1 small AI feature max, not 3 |
| **AWS Solutions Architect cert** | Study time better spent on DSA + applications |
| **M14 K8s, M15 gRPC** | Interview buzzwords only; 2-hour read, not projects |
| **M11 pprof deep dive** | k6 on one project is enough |
| **M16 full system design pack** | 3 classic problems only (URL shortener, rate limiter, job queue) |
| **M8 networking labs bundle** | Read HTTP/TCP/DNS; skip lab bundle |
| **50 micro-projects** | Do 8; skip generic exercises unless they unblock a flagship |
| **Lambda, CloudFront, Route 53 deep dives** | One deploy path only |
| **OpenTelemetry + Jaeger** | Logs + one k6 table in README is enough |
| **5 flagship requirement** | 2 excellent > 5 half-done |

---

## The 8 Projects That Matter

| # | Project | Purpose | Live? |
|---|---------|---------|-------|
| 1 | Git workflow repo | Prove Git fluency | GitHub only |
| 2 | `cli-todo` or small Go CLI | Learn Go syntax | GitHub only |
| 3 | **`jobtrackr` v1** | In-memory REST API | No |
| 4 | **`jobtrackr` v2** | Postgres + JWT + Docker | **Yes — month 4** |
| 5 | **`vaultdrop` lite** | Second live proof (files or webhooks-lite) | **Yes — month 5** |
| 6 | `jobtrackr` on AWS | Same project, cloud deploy | **Yes — month 5** |
| 7 | CI pipeline (GitHub Actions) | lint + test on push | GitHub only |
| 8 | Optional 3rd project | Only if 50+ apps, no callbacks | **Maybe month 7** |

Everything else = **bonus**, not plan.

---

## Month-by-Month Success Criteria

Assuming **start now**, graduation ~**May 2027** (adjust dates if needed).

---

### Month 1 — Foundation + Go basics
**Hours:** 30/week (20 build, 6 course concepts, 4 DSA)

**Build:**
- Git workflow repo done  
- Go tour + `cli-todo`  
- Start `jobtrackr` in-memory (companies, applications, stages)

**Course (watch, implement in Go):**
- Welcome/Setup, Webservers, Backend Systems intro  
- API Development Part One (status codes, POST, validation)

**DSA:** Arrays, hashmaps, two pointers — 15 Easy problems in Go

**Success criteria (must hit all):**
- [ ] GitHub has 2 repos with clean commit history  
- [ ] Can explain request → handler → response without notes  
- [ ] `jobtrackr` runs locally with CRUD on in-memory store  
- [ ] 15 DSA problems done  

**Do NOT:** Start AWS, Docker, AI, or second flagship.

---

### Month 2 — API hardening + Postgres
**Build:**
- `jobtrackr` → Postgres + migrations  
- Middleware: logging, auth stub, error handling  
- Schema: users, companies, applications (ERD drawn)

**Course:**
- API Development Part Two (routers, middleware)  
- All database modules + ERD homework (for your schema)

**DSA:** Stacks, queues, binary search — 15 more Easy/Medium

**Success criteria:**
- [ ] Postgres schema with FK relationships documented  
- [ ] `go test ./...` passes with ≥5 tests  
- [ ] Can write JOIN query and explain normalization  
- [ ] README explains data model  

**Do NOT:** Deploy yet. No Redis unless caching is actually used.

---

### Month 3 — Auth + Docker
**Build:**
- JWT register/login + protected routes  
- RBAC: user owns their applications only  
- Docker Compose: app + Postgres  
- Security pass: parameterized queries only

**Course:**
- Cookies/Session (concept), JWT modules, API Security (SQL injection), CORS

**DSA:** Sliding window, linked list — 15 problems

**Success criteria:**
- [ ] Auth flow works end-to-end in Docker  
- [ ] Invalid/missing JWT returns 401  
- [ ] Can explain JWT vs sessions + bcrypt vs plain hash  
- [ ] `docker compose up` is one command in README  

**Do NOT:** AWS. No second project yet.

---

### Month 4 — Deploy #1 + START APPLYING
**Build:**
- Deploy `jobtrackr` live (pick **one**: Railway/Render/Fly.io **or** EC2 — don’t do both)  
- HTTPS working  
- Add pagination to list endpoints  
- Resume v1 + LinkedIn live

**Course:**
- Response formatting & pagination  
- Beyond CRUD (PUT/PATCH, soft delete)

**Job hunt (starts NOW):**
- 8 applications/week  
- Track every app **inside jobtrackr**  
- 5 outreach messages/week  
- LinkedIn post: “Shipped jobtrackr — live link”

**DSA:** Trees basics, 10 Medium problems

**Success criteria:**
- [ ] **Live URL** for jobtrackr in README  
- [ ] Resume + LinkedIn published  
- [ ] ≥32 applications sent  
- [ ] ≥20 outreach messages sent  
- [ ] 1 mock interview (even self-recorded)  

**This is the most important month.** If you miss live URL + applications, v2.1 fails.

---

### Month 5 — Second flagship + AWS lite + volume apply
**Build:**
- **`vaultdrop` lite:** auth + file upload + expiring share links (S3 or MinIO locally → S3 on AWS)  
- Move `jobtrackr` to AWS if not already (RDS + ECS or EC2 — one path)  
- GitHub Actions: test on every push  
- k6 smoke test on `jobtrackr`; P95 in README

**Course:**
- File uploader module (concepts only)  
- Load testing with k6 (one test script)

**Job hunt:**
- **10–12 applications/week**  
- 5 outreach/week  
- Apply to: intern, junior backend, contract, “backend Go”, “backend remote”  
- Optional: port `jobtrackr` to Express in **one weekend** for BD/Node keyword roles

**DSA:** 2 Medium problems/week; focus patterns you’ve seen in apps

**Success criteria:**
- [ ] **2 live URLs** pinned on GitHub  
- [ ] CI green on main branch  
- [ ] k6 numbers in at least one README  
- [ ] ≥80 total applications  
- [ ] ≥2 recruiter/hiring manager replies (any outcome)  
- [ ] DECISIONS.md on both projects (≥3 entries each)  

**Do NOT:** Start `taka-flow`, RAG, or `pulsewatch`.

---

### Month 6 — Interview mode + optional 3rd project
**Build (pick ONE):**
- **Option A (recommended):** Polish existing 2 projects (OpenAPI, better README, fix bugs from self-use)  
- **Option B:** Small `hookrelay` lite (webhook receiver + retry queue) — only if callbacks are zero  
- **Option C:** One tiny AI feature on jobtrackr (paste job URL → structured JSON extract) — 1 week max

**Job hunt:**
- 10 applications/week (quality over quantity if interviewing)  
- 3 mock interviews/month  
- 1 technical article: “How I built jobtrackr” or “JWT + Postgres in Go”  
- Pursue **any** intern/contract: Upwork, Contra, local startup

**DSA:** Daily if interviewing; 1 Medium/day otherwise

**Success criteria:**
- [ ] ≥3 first-round interviews **OR** ≥1 intern/contract offer  
- [ ] Can pitch jobtrackr in 3 minutes without slides  
- [ ] Can defend 3 DECISIONS.md entries aloud  
- [ ] 1 published article or detailed LinkedIn post  

---

### Month 7 — Graduation runway (Feb 2027 if started Jul 2026)
**Build:** Maintenance only unless interviews demand something specific

**Job hunt:**
- Full-time application push: 12/week  
- Follow up on all “Applied” rows in jobtrackr  
- Ask for referrals from anyone who replied  
- Target BD internationally-focused companies (stepping stone)

**Success criteria:**
- [ ] ≥150 total applications tracked  
- [ ] ≥5 completed interview processes (pass or fail)  
- [ ] ≥1 offer (any: intern, contract, hybrid, remote) **OR** final-round at 2+ companies  

---

### Month 8–10 — Until graduation / offer
**If offer secured:** Take it. Learn K8s/gRPC/taka-flow **on the job or after hours**.

**If no offer yet:**
- Cut all new building  
- 100% focus: applications, referrals, DSA, mocks  
- Consider 3-month local intern at any backend stack  
- Revisit Node/Python port for BD market  

**Success criteria by graduation:**
- [ ] **Offer in hand** (ideal)  
- [ ] OR strong pipeline (2+ final rounds) + intern/contract experience  

---

## Minimum “Can I Apply?” Checklist (End of Month 3 / Start of Month 4)

You need **all** of these:

- [ ] Go: variables, structs, interfaces, error handling, basic concurrency  
- [ ] REST API with proper status codes and validation  
- [ ] Postgres: schema, migrations, JOINs, transactions  
- [ ] JWT + bcrypt + user-scoped data  
- [ ] Docker Compose runs locally  
- [ ] Tests exist and pass  
- [ ] Git history looks human (not one giant commit)  
- [ ] README: setup, architecture, env vars  
- [ ] DSA: ~45 problems done  

You do **not** need: AWS, Redis, RAG, K8s, gRPC, 5 projects, cert.

---

## Weekly Time Split (30 hrs)

| Activity | Hrs/week | From |
|----------|----------|------|
| Building | 14–16 | Month 1 |
| Instructor course (concept → Go) | 4–5 | Month 1–5 |
| DSA | 5–8 | Month 1+ |
| Applications + outreach | 2 | Month 4+ |
| Applications + outreach | 6–8 | Month 5+ |
| Mock interviews / articles | 2–4 | Month 6+ |

When job hunt ramps, **steal from building**, not from DSA.

---

## Application Strategy (Remote Fresher from BD)

**Search titles (not just “Go Developer”):**
- Backend intern  
- Software engineer intern remote  
- Junior backend engineer  
- Platform engineer intern  
- Go backend intern  

**Boards:** Wellfound, RemoteOK, Remotive, Himalayas, Remote Rocketship, Golang Cafe, LinkedIn (remote filter), Bdjobs/Niyog (backup)

**Every application includes:**
1. Live URL (jobtrackr)  
2. GitHub link  
3. 2 sentences: problem you solved + one trade-off (JWT vs session, etc.)

**Accept as win:**
- Remote contract (3–6 months)  
- Local intern at company with international clients  
- Part-time backend gig  

These unlock “1 year experience” filters faster than a fifth flagship.

---

## What “Success” Looks Like (Honest)

| Timeline | Realistic win |
|----------|----------------|
| Month 4 | 1 live project + applying |
| Month 5 | 2 live projects + 80 apps + some replies |
| Month 6–7 | Interviews + maybe intern/contract |
| Month 8–10 | **First offer** (remote ideal; local OK) |

**v2.1 success metric:** Offer or paid intern by graduation — **not** “finished 24 modules.”

---

## v2.1 One-Page Summary

```
MONTH 1-3:  Build jobtrackr (local → Postgres → auth → Docker)
MONTH 4:    Deploy jobtrackr + START APPLYING (8/week)
MONTH 5:    Deploy vaultdrop lite + AWS + CI + APPLY HARD (10-12/week)
MONTH 6:    Interview prep + polish OR tiny 3rd project if zero callbacks
MONTH 7-10: Offers > building

KEEP:   jobtrackr, vaultdrop lite, Git, Go, SQL, JWT, Docker, 1 cloud deploy, DSA, applications
CUT:    taka-flow, pulsewatch, full AI/RAG, K8s, gRPC, AWS cert, 3 extra flagships
```

---

## If You Slip Behind Schedule

**Cut in this order:**
1. vaultdrop → simplify to “second CRUD API with one unique feature”  
2. AWS → stay on Railway/Render  
3. AI feature → delete  
4. CI/CD → manual deploy OK for month 4–5  
5. **Never cut:** live URL, applications, DSA  

**Never extend “start applying” past month 5.**

---

I'm in **Ask mode**, so this is text only. If you want this saved as `Go_backend_v2.1_remote_fresher.md` in your repo (and optionally trimmed sections merged into your existing v2 doc), switch to **Agent mode** and ask me to write the file.
