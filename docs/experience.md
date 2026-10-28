# Engineering experience — Dilshod Mahmudov

This is the longer technical background behind my [GitHub profile](../README.md). The focus is on **work I have personally contributed to**, not a list of technologies I've only read about.

## Poputi — Software Developer

**Aug 2026 – Present · Dushanbe, Tajikistan**  
Product: [poputi.tj](https://poputi.tj/ru)

Poputi is a carpooling and transport platform with a Go backend and web/mobile clients. Working in an inherited codebase taught me that understanding what is actually running is often the most important first step.

My work has included:

- Comparing development branches, deployed application behavior, and historical changes.
- Examining PostgreSQL schema and migration state to understand inconsistencies.
- Working on a production Linux machine through SSH.
- Creating application backups and performing binary deployments.
- Managing and verifying `systemd` services.
- Reviewing Nginx and application runtime configuration.
- Using logs, database state, and service behavior to investigate failures.
- Establishing a safer baseline for subsequent development.

The central lesson: **a successful local build is not proof that the deployed service, configuration, and database agree**.

## Hadaf — Backend Developer

**2025 – Present · Remote**

Hadaf connects donors with institutions and individuals seeking support. I contribute to an existing Go backend organized into handlers, services, repositories, models, and middleware.

Selected contributions:

- Implemented REST API functionality and integrated it into the project codebase.
- Built Go `httptest` integration tests for registration, OTP confirmation, login, and protected endpoints.
- Implemented Telegram notification behavior for application panics and HTTP 5xx responses, designed not to take down request handling when alert delivery fails.
- Worked with PostgreSQL, Redis, MinIO, Docker Compose, JWT, and rate limiting.
- Participated in debugging, testing, and code review.

## Tcell Mentor Program — Backend Developer Intern

**May – Oct 2025 · Dushanbe, Tajikistan**

Backend development practice under mentor supervision:

- Go CRUD services and REST APIs.
- gRPC and Protocol Buffers.
- PostgreSQL/SQLite relational schemas, SQL, and GORM.
- JWT authentication, password hashing, and migrations.
- API testing, Docker, Git workflows, and debugging.

## Public technical projects

### [University Academic Records System](https://github.com/Human-Unit/MSU_tables)

Desktop software for university workflows, using Go/Wails, PostgreSQL/GORM, React, and TypeScript.

Implemented areas include faculties, groups, students, teachers, subjects, classrooms, attendance, performance, examinations, teacher workload, and weekly schedules. The project also has database migrations, seed data, soft deletion, cascading academic filters, and Russian/English UI support.

### [SolidSnakeBot](https://github.com/Human-Unit/SolidSnakeBot)

A Python Telegram bot using local inference through LM Studio's OpenAI-compatible API. It supports retrieval over local notes via Sentence Transformers and FAISS, opt-in DuckDuckGo search, external currency data, configurable prompts, and per-user chat history.

### [Student Council Website](https://github.com/Human-Unit/Student_Council)

A Next.js/TypeScript website developed around an existing university student-council brand system, with reusable content data and design components. This complements my student-council communications and visual-review work.

### [Predator's Vision](https://github.com/Human-Unit/Predator-s-Vision)

An experimental Python/OpenCV computer-vision project with a science-fiction-inspired HUD.

## Other product experience

**Navruz — manual QA and product review.** My contribution centered on testing user flows, finding visual inconsistencies, correcting user-facing text, reviewing visual materials, and suggesting UX improvements. I was **not** the primary developer.

## How I investigate a backend problem

1. **Reproduce and describe** the failure: request, response, environment, and expected behavior.
2. **Inspect the running system:** logs, deployment configuration, service state, environment differences, and infrastructure.
3. **Trace the data path:** API handler, service logic, database schema, and migration history.
4. **Limit the change:** prefer an explainable, minimal fix over an unrelated rewrite.
5. **Verify:** tests, targeted manual checks, and post-deployment runtime observations.

## Technical focus

- **Go services:** Gin, REST, gRPC, Protocol Buffers, GORM, middleware, JWT/RBAC.
- **Data:** PostgreSQL, SQLite, Redis, MinIO, migrations, schema debugging.
- **Infrastructure:** Linux, SSH, Docker/Compose, Nginx, systemd, backups, deployments.
- **Testing:** Go's `testing` and `httptest`, API/integration testing, manual QA.
- **Exploration:** Python, C++, local LLMs, RAG, FAISS, Telegram integrations.

I am particularly interested in teams working on **Go backends, APIs, reliability, databases, and automation**.

[Back to the profile](../README.md)
