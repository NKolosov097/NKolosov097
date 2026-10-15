# Nikita Kolosov

Software Engineer building web, mobile, and backend systems in **TypeScript,
Python, and Go**.

On the front I work with React, React Native, and Next.js; behind them I write
services in Node.js, FastAPI, and Go, backed by PostgreSQL and MongoDB. I care
about architecture, real-time experiences, authentication and security, testing,
accessibility, and performance — and about shipping: Docker, CI/CD, and cloud
deployment are part of the job, not an afterthought.

I also have commercial experience integrating AI providers into production
applications, including user-facing AI workflows, API integration, error handling,
and reliability concerns. Further implementation details are confidential under NDA;
[Clinical Cases](https://github.com/NKolosov097/clinical-cases) below is a public
example of how I approach it.

[Portfolio](https://nkolosov.com) ·
[CV](https://nkolosov.com/assets/cv/cv-nikita-kolosov.pdf) ·
[Email](mailto:NKolosov097@gmail.com)

## Featured projects

### [Clinical Cases](https://github.com/NKolosov097/clinical-cases)

A full-stack clinical-case trainer: an author turns free clinical text into a
structured case with Gemini-assisted extraction, a learner answers, and grading
is deterministic.

- FastAPI, SQLAlchemy 2, Alembic, and PostgreSQL 17 behind Next.js 16 Server Components
- Gemini structured output validated with Pydantic; grading is exact-match against a human-supplied reference, never an LLM judgment call
- TypeScript types generated from the OpenAPI contract, with CI failing on drift
- pytest, mypy, Vitest, Playwright, and pixel-diff screenshot regression
- Deployed to Cloud Run and Cloud SQL with OpenTelemetry tracing

[Live demo](https://eximion-frontend-497115726994.europe-west3.run.app) ·
[Source code](https://github.com/NKolosov097/clinical-cases)

### [Auth Service](https://github.com/NKolosov097/auth-service)

An authentication microservice in Go over a JSON HTTP API, written with the
threat model in mind rather than the happy path.

- Email/password, Google OAuth2 (OpenID Connect), and Telegram Login Widget
- Short-lived JWT access tokens with rotating refresh tokens, stored only as SHA-256 hashes
- Password reset and email change via expiring confirmation links
- Per-IP rate limiting, request and header size limits, security headers on every response
- Structured logging with `log/slog`, graceful shutdown, PostgreSQL migrations

[Source code](https://github.com/NKolosov097/auth-service)

### [NK Meet](https://github.com/NKolosov097/nk-meet)

A cross-platform video meeting application built with React Native, Expo,
TypeScript, and LiveKit.

- Real-time audio and video communication
- Native Android and iOS development builds
- Typed room state, validation, and user-facing error handling
- Accessibility support and integration tests

[Source code](https://github.com/NKolosov097/nk-meet)

### [Portfolio](https://nkolosov.com)

A production-oriented personal website built with Next.js, React, and strict
TypeScript—not just a landing page, but a tested full-stack application.

- Server-first contact flow with Zod, PostgreSQL, Prisma, and transactional email
- English and Russian localization
- Unit and Playwright end-to-end tests
- Accessibility, responsive rendering, SEO, and performance-conscious animation
- Health endpoint and deployment-ready configuration

[Live site](https://nkolosov.com) ·
[Source code](https://github.com/NKolosov097/portfolio)

### [Protein](https://github.com/NKolosov097/protein-web)

An interactive 3D browser game built around real cancer-related protein
structures loaded from the Protein Data Bank.

- Six real molecular targets rendered in 3D
- Desktop and mobile gesture controls with adaptive graphics
- Guided onboarding, study mode, and bilingual UI
- Browser-based scoring with an optional FastAPI backend

[Live demo](https://nkolosov097.github.io/protein-web/) ·
[Source code](https://github.com/NKolosov097/protein-web)

## Engineering strengths

- **Web:** React, Next.js, TypeScript, Server Components, accessible and responsive interfaces
- **Mobile:** React Native, Expo, native integrations, real-time audio and video
- **Backend:** Node.js, Python (FastAPI), Go, REST and OpenAPI design, validation, background and server-side workflows
- **Data:** PostgreSQL, MongoDB, Prisma, Drizzle, SQLAlchemy, schema migrations
- **Auth and security:** JWT with refresh rotation, OAuth2 and OpenID Connect, password hashing, rate limiting, secret handling
- **AI integrations:** third-party AI providers, structured and validated model output, user-facing AI workflows, resilient error handling
- **Quality:** unit, integration, and end-to-end testing; strict typing; static analysis; code review
- **Delivery:** Docker, CI/CD, Cloud Run, Vercel, Linux, observability and structured logging
- **Product:** internationalization and RTL layouts, payment flows, SEO, performance budgets

## A little more about me

I have been building software professionally since 2021. Outside engineering,
I spend time with my Labrador and enjoy motorcycles.

If you are building a web or mobile product and think I could help,
[send me an email](mailto:NKolosov097@gmail.com).
