# Mert Seker

I build the backend plumbing that makes LLM agents dependable: durable job pipelines, multi-tenant Postgres, idempotent workers, the human review loops that tell you whether a prompt change actually helped, and the guardrails that keep coding agents out of production.

Final-year BSc Computing (Artificial Intelligence) at the University of Greenwich, London.

## Open source

| Project | What it is |
|---|---|
| [offlimits](https://github.com/meertseker/offlimits) | The hook that keeps your coding agent out of production. A Claude Code plugin that blocks pushes to protected branches, remote migrations, deploys and production database writes from agent sessions, even when they run with `--dangerously-skip-permissions`. |
| [evalroom](https://github.com/meertseker/evalroom) | Human-in-the-loop quality control for LLM outputs. Multi-lens review, versioned rubrics, inter-rater agreement, golden sets and gated regression runs. No bare pass rate ever leaves. |
| [durastep](https://github.com/meertseker/durastep) | Durable, idempotent multi-step agent pipelines on your own Postgres and Redis. Typed worker registry, DAG chains, race-safe scheduling, error taxonomy, deadlines, quotas, stuck-run recovery. |

offlimits is the gate hook from the coordinator/worker agent setup I run on a production school-management system, made general. evalroom and durastep were extracted from a production sales-intelligence pipeline I led for six months, then rebuilt as dependency-light libraries with the domain removed.

## Systems I've built

- **seker-platform** (private): the public website and the staff CRM of a kindergarten in Istanbul, in one monorepo. A parent's application on the site opens as a candidate card in the CRM, enrolments carry their instalment plans, and enrolments that came from Google Ads are uploaded back to the ad account as conversions. Next.js, Supabase Postgres with row-level security on every table, nightly database backups to S3. Built alone.
- **[logistic-comp-order-tracking-system](https://github.com/meertseker/logistic-comp-order-tracking-system)**: offline-first desktop app that tracks orders and prices every trip for a logistics company in Istanbul: fuel, driver days, tolls and maintenance per vehicle, with cost snapshots kept per order. Electron, React and SQLite, auto-updates from GitHub Releases, Windows and macOS installers built in CI.
- **Sekersoft** (2024 to 2026, solo): built `sekersoft-erp-core` (private), a multi-tenant ERP engine (NestJS, PostgreSQL, tenant isolation, TOTP 2FA, field-level encryption, 60+ granular permissions, transactional outbox). Every ERP I shipped to clients runs on top of it.
- **Revint** (2026, co-founder and lead engineer): LLM pipeline that researched local businesses and produced a sales decision per lead, with a three-lens human review room to measure it. Discontinued in October 2026; evalroom and durastep come from it.

## Research

Dissertation (2026 to 2027): independent evaluation of coding-agent add-ons, separating what the model does from what the harness does. Built on evalroom for the review statistics and durastep for running the experiment matrix, so the dissertation ships with both libraries.

## Stack

TypeScript, Node.js, NestJS, PostgreSQL, Redis and BullMQ, Prisma, Next.js, Supabase, Electron. Python for evaluation work.

## Contact

[LinkedIn](https://www.linkedin.com/in/mertseker) · meertseker@gmail.com
