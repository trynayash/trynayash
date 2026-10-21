# Yash Suthar

Software engineer in Mumbai. I build products end to end: React front ends, Go and Node.js APIs, PostgreSQL and Redis, and the CI/CD and AWS setup they run on.

Looking for software engineering roles in backend, full stack or platform, remote or on-site.

[Portfolio](https://www.yashsuthar.dev) · [Resume](https://www.yashsuthar.dev/resume.pdf) · [Email](mailto:hello@yashsuthar.dev)

## Work

### [LimitYourAPI](https://limityourapi.tech)

API rate limiting as a service. I built and deployed it on my own.

- Go (Gin) API where each limit decision is one atomic Redis Lua script: token bucket, sliding window, quota and token cost.
- React dashboard with API keys, organizations and two-factor login.
- Node.js SDK on npm, Go and Python SDKs, and a Cloudflare Workers limiter that enforces signed rule snapshots at the edge.
- GitHub Actions CI runs Go tests with the race detector, govulncheck and the frontend build. The API runs on Render and the dashboard on Vercel.

Go, Redis, Lua, React, PostgreSQL, Cloudflare Workers · [Case study](https://www.yashsuthar.dev/work/limityourapi) · [SDK](https://github.com/trynayash/limityourapi-sdk)

### [StartupDeckAI](https://www.startupdeck.in)

A live web app that helps founders test startup ideas. About 200 people signed up and ran more than 1,000 analyses by October 2026.

- React and TypeScript front end, Express API that streams each analysis over SSE, PostgreSQL and Razorpay subscriptions.
- Four AI stages run in parallel, then a synthesis stage, and a fixed scoring formula gives a GO, PIVOT or KILL verdict. Every number in a report says where it came from.
- Every push runs lint, type checks and 3,400+ tests (Vitest and Playwright) in GitHub Actions, and a passing run on main deploys the API.
- BullMQ workers on Redis send email and run scheduled jobs.

React, TypeScript, Node.js, PostgreSQL, Redis · [Case study](https://www.yashsuthar.dev/work/startupdeck)

### [ScopeCI](https://github.com/trynayash/scopecihq)

A tool I'm building for software agencies: it checks each pull request against the scope the client signed. In development, with a waitlist open. [Case study](https://www.yashsuthar.dev/work/scopeci)

## Research

[Overshoot, Retries and Clocks: An Empirical Study of Redis-Based Rate Limiting Under Concurrency](https://doi.org/10.5281/zenodo.23467402) (preprint, October 2026)

I tested 8 Redis rate limiters in 3,853 trials. Check-then-act let through 29% too many requests at 64 workers, WATCH/MULTI turned away up to 42% of valid requests, and trusting the caller's clock cut a token bucket to 16% of its rate. The code and data are public. [Summary](https://www.yashsuthar.dev/writing/redis-rate-limiter-failures-measured)

Follow-up: [Atomic rate limiting with Redis and Lua, measured](https://www.yashsuthar.dev/writing/atomic-rate-limiting-redis-lua)

## Stack

- **Languages:** Go, TypeScript, JavaScript, Python, SQL
- **Front end:** React, Vite, Tailwind CSS, TanStack Query
- **Back end:** Node.js, Express, Gin, GraphQL, REST, WebSockets
- **Data:** PostgreSQL, Redis, MongoDB
- **Infrastructure and testing:** Docker, Terraform, GitHub Actions, Render, Vercel, Cloudflare Workers, Linux, Vitest, Playwright

## Experience

- Founder and software engineer, LimitYourAPI (2026 to now) and StartupDeckAI (2025 to now)
- Lab Technician Intern, Parul University computer lab (2023): set up and maintained 120+ systems and fixed 15+ issues a day

## Education

- MCA, Late Bhausaheb Hiray S.S. Trust's Institute of Computer Applications, Mumbai (2025 to 2027, CGPA 8.83)
- BCA, Parul University, Vadodara (2022 to 2025, CGPA 7.93)
