# Yash Suthar

Software engineer in Mumbai. I build products end to end: React front ends, Go and Node.js APIs, PostgreSQL and Redis, and the CI/CD and AWS setup they run on.

Looking for software engineering roles in backend, full stack or platform, remote or on-site.

[Portfolio](https://www.yashsuthar.dev) · [Resume](https://www.yashsuthar.dev/resume.pdf) · [Email](mailto:hello@yashsuthar.dev)

## Work

### [LimitYourAPI](https://limityourapi.tech)

API rate limiting as a service. I built and launched it on my own.

- Go API where every limit check is one atomic Redis Lua call, measured at 6 to 14 µs of Redis CPU per check.
- React dashboard with API keys, organizations, two-factor login and Stripe billing.
- SDKs for Node.js, Go and Python, and a Cloudflare Workers limiter that runs at the edge.
- GitHub Actions deploys to AWS ECS Fargate, with the infrastructure written in Terraform.

Go, Redis, Lua, React, PostgreSQL, AWS, Terraform · [Case study](https://www.yashsuthar.dev/work/limityourapi) · [SDK](https://github.com/trynayash/limityourapi-sdk)

### [StartupDeckAI](https://www.startupdeck.in)

A live web app that helps founders test startup ideas, used by 214+ people.

- React and TypeScript front end, Express and GraphQL API, PostgreSQL.
- Four AI stages and a synthesis stage feed a fixed scoring formula that gives a GO, PIVOT or KILL verdict. Every number in a report says where it came from.
- Slow AI work runs in BullMQ workers on Redis, with leases, so a restart or a deploy doesn't leave a job stuck.
- 3,400+ tests (Vitest and Playwright) run in GitHub Actions before every deploy.

React, TypeScript, Node.js, GraphQL, PostgreSQL, Redis · [Case study](https://www.yashsuthar.dev/work/startupdeck)

### [ScopeCI](https://github.com/trynayash/scopecihq)

CI/CD for software agencies that checks each change against the client contract before it ships. Early stage, waitlist open. [Case study](https://www.yashsuthar.dev/work/scopeci)

## Research

[Overshoot, Retries and Clocks: An Empirical Study of Redis-Based Rate Limiting Under Concurrency](https://doi.org/10.5281/zenodo.23467402) (preprint, October 2026)

I tested 8 Redis rate limiters in 3,853 trials. Check-then-act let through 29% too many requests at 64 workers, WATCH/MULTI turned away up to 42% of valid requests, and trusting the caller's clock cut a token bucket to 16% of its rate. The code and data are public. [Summary](https://www.yashsuthar.dev/writing/redis-rate-limiter-failures-measured)

Follow-up: [Atomic rate limiting with Redis and Lua, measured](https://www.yashsuthar.dev/writing/atomic-rate-limiting-redis-lua)

## Stack

- **Languages:** Go, TypeScript, JavaScript, Python, SQL
- **Front end:** React, Vite, Tailwind CSS, TanStack Query
- **Back end:** Node.js, Express, Gin, GraphQL, REST, WebSockets
- **Data:** PostgreSQL, Redis, MongoDB
- **Infrastructure and testing:** Docker, AWS, Terraform, GitHub Actions, Vercel, Linux, Vitest, Playwright

## Education

- MCA, Late Bhausaheb Hiray S.S. Trust's Institute of Computer Applications, Mumbai (2025 to 2027, CGPA 8.83)
- BCA, Parul University, Vadodara (2022 to 2025, CGPA 7.93)
