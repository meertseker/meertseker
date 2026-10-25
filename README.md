# Mert Seker

Final-year BSc Artificial Intelligence student in London. I build the backend plumbing that makes LLM agents dependable: job pipelines, multi-tenant Postgres, idempotent workers, and the human review loops that tell you whether a prompt change actually helped.

## Open source

| Project | What it is |
|---|---|
| [evalroom](https://github.com/meertseker/evalroom) | Human-in-the-loop quality control for LLM outputs. Multi-lens review, versioned rubrics, inter-rater agreement, golden sets and gated regression runs. No bare pass rate ever leaves. |
| [durastep](https://github.com/meertseker/durastep) | Durable, idempotent multi-step agent pipelines on your own Postgres and Redis. Typed worker registry, DAG chains, race-safe scheduling, error taxonomy, deadlines, quotas, stuck-run recovery. |

Both were extracted from a production sales-intelligence pipeline I led for six months, then rebuilt as dependency-light libraries with the domain removed.

## Background

- Lead engineer and founder at Revint (2026): LLM pipeline that researched local businesses and produced a sales decision per lead, with a three-lens human review room to measure it. Discontinued in October 2026.
- Solo engineer at Sekersoft (2024 to 2026): a multi-tenant clinic ERP (NestJS, PostgreSQL, field-level encryption, transactional outbox) and an offline-first logistics desktop app (Electron, SQLite), both still in daily use.
- Dissertation (2026 to 2027): independent evaluation of coding-agent add-ons, separating what the model does from what the harness does.

## Stack

TypeScript, Node.js, PostgreSQL, Redis and BullMQ, Prisma, Next.js, Python for evaluation work.

## Contact

[LinkedIn](https://www.linkedin.com/in/mertseker) · meertseker@gmail.com
