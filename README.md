<div align="center">

<br/>

<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
<img alt="React" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=white"/>
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
<img alt="Go" src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white"/>
<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img alt="Redis" src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>
<img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>

<br/>
<br/>

<a href="https://www.yashsuthar.dev">
  <img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-020617?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>

<a href="https://www.yashsuthar.dev/resume.pdf">
  <img alt="Resume" src="https://img.shields.io/badge/Resume-111827?style=for-the-badge"/>
</a>

<a href="mailto:hello@yashsuthar.dev">
  <img alt="Email" src="https://img.shields.io/badge/Email-1E293B?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<br/>
<br/>

<img alt="Profile views" src="https://komarev.com/ghpvc/?username=trynayash&label=Profile+Views&color=111827&style=flat-square"/>

</div>

---

## About

Software engineer in Mumbai. I build and ship complete products: the interface, the API, the data model, the tests, and the CI/CD and cloud infrastructure they run on. Founder of LimitYourAPI, ScopeCI and StartupDeckAI.

```ts
const yash = {
  role: "Software Engineer (full stack)",
  location: "Mumbai, India",

  stack: {
    frontend: ["React", "TypeScript", "Vite", "Tailwind CSS"],
    backend: ["Node.js", "Express", "Go", "GraphQL"],
    data: ["PostgreSQL", "Redis", "MongoDB"],
    delivery: ["Docker", "Terraform", "AWS", "GitHub Actions"],
  },

  shipped: ["LimitYourAPI", "StartupDeckAI", "ScopeCI"],

  openTo: ["Full stack", "Backend", "Frontend", "Platform and DevOps"],
}
```

---

## Engineering Principles

| Principle | Approach |
|:--|:--|
| **Design Before Code** | The data model, the user flow and the failure modes come first. |
| **Fast for the User** | Page weight, API latency and query cost are budgets from day one. |
| **Boring Where It Counts** | React, PostgreSQL, Redis, plain HTTP and Docker unless the problem demands otherwise. |
| **Tested and Shipped Often** | Type checks, tests and CI on every change, with automated deploys. |

---

## Tech Stack

### Languages

<img alt="TypeScript, JavaScript, Go, Python, Java, C, HTML, CSS" src="https://skillicons.dev/icons?i=ts,js,go,python,java,c,html,css&theme=dark"/>

### Frontend

<img alt="React, Vite, Tailwind CSS" src="https://skillicons.dev/icons?i=react,vite,tailwind&theme=dark"/>

### Backend & Data

<img alt="Node.js, Express, GraphQL, PostgreSQL, Redis, MongoDB" src="https://skillicons.dev/icons?i=nodejs,express,graphql,postgres,redis,mongodb&theme=dark"/>

### DevOps & Testing

<img alt="Docker, AWS, Terraform, GitHub Actions, Vercel, Linux, Vitest" src="https://skillicons.dev/icons?i=docker,aws,terraform,githubactions,vercel,linux,vitest&theme=dark"/>

---

## Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### LimitYourAPI

API rate limiting SaaS, built and launched end to end.

**Highlights:**

- Go API where every limit is one atomic Redis Lua call
- 6–14 µs of Redis CPU per check, measured
- React dashboard, API keys, TOTP 2FA, Stripe billing
- SDKs for Node.js, Go and Python
- GitHub Actions CI/CD to AWS ECS Fargate, infrastructure in Terraform

**Stack**
`Go` `React` `Redis` `PostgreSQL` `Terraform` `AWS`

<a href="https://limityourapi.tech">
  <img alt="Live" src="https://img.shields.io/badge/Live-020617?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>

<a href="https://www.yashsuthar.dev/work/limityourapi">
  <img alt="Case Study" src="https://img.shields.io/badge/Case_Study-111827?style=for-the-badge"/>
</a>

<a href="https://github.com/trynayash/limityourapi-sdk">
  <img alt="SDK" src="https://img.shields.io/badge/SDK-1E293B?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</td>

<td width="50%" valign="top">

### StartupDeckAI

Live AI SaaS with 214+ users, built end to end.

**Highlights:**

- React and TypeScript UI with TanStack Query and Tailwind CSS
- Express and GraphQL API on PostgreSQL
- Four parallel LLM stages feed a deterministic 8-dimension score
- Slow generation runs in BullMQ workers on Redis
- 3,400+ tests run in CI before every deploy

**Stack**
`React` `TypeScript` `Node.js` `GraphQL` `PostgreSQL` `BullMQ`

<a href="https://www.startupdeck.in">
  <img alt="Live" src="https://img.shields.io/badge/Live-020617?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>

<a href="https://www.yashsuthar.dev/work/startupdeck">
  <img alt="Case Study" src="https://img.shields.io/badge/Case_Study-111827?style=for-the-badge"/>
</a>

</td>
</tr>

<tr>
<td width="50%" valign="top">

### PromptP

Real-time event-driven platform.

**Highlights:**

- Append-only Redis Streams log as the single source of truth
- Every client view is derived from the log
- Per-socket backpressure
- Reconnects resume from the client's last event

**Stack**
`Node.js` `Redis Streams` `WebSockets` `React`

<a href="https://www.yashsuthar.dev/work/promptp">
  <img alt="Case Study" src="https://img.shields.io/badge/Case_Study-111827?style=for-the-badge"/>
</a>

<a href="https://github.com/trynayash/promptp">
  <img alt="Repository" src="https://img.shields.io/badge/Repository-1E293B?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</td>

<td width="50%" valign="top">

### CodeFusionAI

Collaborative coding environment.

**Highlights:**

- Operational Transformation for concurrent editing
- Per-session Docker sandboxes with cgroup CPU and memory limits
- Presence on its own channel, separate from document traffic

**Stack**
`Go` `Docker` `WebSockets` `React`

<a href="https://www.yashsuthar.dev/work/codefusionai">
  <img alt="Case Study" src="https://img.shields.io/badge/Case_Study-111827?style=for-the-badge"/>
</a>

<a href="https://github.com/trynayash/codefusionai">
  <img alt="Repository" src="https://img.shields.io/badge/Repository-1E293B?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</td>
</tr>
</table>

Also building **ScopeCI**: CI/CD for software agencies that ties the client contract and the project tracker to GitHub workflows, so unapproved work is caught before production. Waitlist open. [Case study](https://www.yashsuthar.dev/work/scopeci) · [GitHub](https://github.com/trynayash/scopecihq)

---

## Research

### Overshoot, Retries and Clocks: An Empirical Study of Redis-Based Rate Limiting Under Concurrency

**Preprint, Zenodo • Oct 2026**<br/>
Tested 8 Redis rate limiters in 3,853 trials. Check-then-act over-admitted 29% at 64 workers, WATCH/MULTI refused up to 42% of valid requests, and caller clocks cut a token bucket to 16% of its rate. Code and data are public.

<a href="https://doi.org/10.5281/zenodo.23467402">
  <img alt="DOI 10.5281/zenodo.23467402" src="https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23467402-020617?style=for-the-badge"/>
</a>

<a href="https://www.yashsuthar.dev/writing/redis-rate-limiter-failures-measured">
  <img alt="Summary" src="https://img.shields.io/badge/Summary-111827?style=for-the-badge"/>
</a>

Follow-up article: [Atomic rate limiting with Redis and Lua, measured](https://www.yashsuthar.dev/writing/atomic-rate-limiting-redis-lua) (7 experiments on Redis 7).

---

## Experience

### Founder & Software Engineer, LimitYourAPI

**Jan 2026 — Present**<br/>
Built and launched an API rate-limiting SaaS end to end: Go API, React dashboard, Stripe billing, SDKs for three languages, and CI/CD to AWS with the infrastructure in Terraform.

### Founder & Software Engineer, StartupDeckAI

**Jan 2025 — Present**<br/>
Built a live AI SaaS (214+ users) end to end: React and TypeScript UI, Express and GraphQL API on PostgreSQL, BullMQ workers, and 3,400+ tests in GitHub Actions before every deploy.

### Founder & Software Engineer, ScopeCI

**2026 — Present**<br/>
Commercial CI/CD for software agencies, connecting the client contract to the code. Waitlist open.

### Lab Technician, Parul University Computer Lab

**2023**<br/>
Deployed and maintained 120+ systems and triaged 15+ issues a day.

---

## Education

### Master of Computer Applications

**Late Bhausaheb Hiray S.S. Trust's Institute of Computer Applications, Mumbai • 2025 — 2027**<br/>
CGPA 8.83/10. Coursework: data structures and algorithms, operating systems, computer networks, distributed systems, system design.

### Bachelor of Computer Applications

**Parul University, Vadodara • 2022 — 2025**<br/>
CGPA 7.93/10.

---

## GitHub Metrics

![GitHub Snake](.github/assets/github-snake-dark.svg)

<br/>

<img alt="GitHub stats" height="180em" src="https://github-readme-stats.shion.dev/api?username=trynayash&show_icons=true&hide_border=true&bg_color=020617&title_color=ffffff&text_color=cbd5e1&icon_color=94a3b8&ring_color=94a3b8"/>

<img alt="Top languages" height="180em" src="https://github-readme-stats.shion.dev/api/top-langs/?username=trynayash&layout=compact&hide_border=true&bg_color=020617&title_color=ffffff&text_color=cbd5e1"/>

<br/>

<img alt="GitHub streak" width="70%" src="https://streak-stats.demolab.com/?user=trynayash&theme=dark&hide_border=true&background=020617&stroke=475569&ring=94A3B8&fire=FFFFFF&currStreakLabel=FFFFFF"/>

<br/>

### Contribution Graph

![GitHub Contribution Graph](https://ghchart.rshah.org/trynayash)

<br/>

### Achievements

🏆 **GitHub Profile Trophy**

<img src="https://github-profile-trophy.vercel.app/?username=trynayash&row=1&column=3&no-bg=true&no-frame=true&theme=dark" alt="GitHub Profile Trophy"/>

---

## Current Focus

```yaml
Building:
  - LimitYourAPI: rate limiting and usage metering for APIs
  - ScopeCI: CI/CD for software agencies
  - StartupDeckAI: AI market analysis and pitch decks for founders

Writing:
  - Measured studies of the systems I build

Looking for:
  - Software engineering roles: full stack, backend, frontend, platform and DevOps
```

---

## Connect

Open to software engineering roles (full stack, backend, frontend, platform and DevOps), remote or in Mumbai.

<br/>

<a href="mailto:hello@yashsuthar.dev">
  <img alt="Email" src="https://img.shields.io/badge/Email-020617?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<a href="https://github.com/trynayash">
  <img alt="GitHub" src="https://img.shields.io/badge/GitHub-111827?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<a href="https://www.yashsuthar.dev">
  <img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-1E293B?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>

<a href="https://www.yashsuthar.dev/resume.pdf">
  <img alt="Resume" src="https://img.shields.io/badge/Resume-020617?style=for-the-badge"/>
</a>

<br/>
<br/>
