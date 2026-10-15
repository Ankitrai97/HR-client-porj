# HR client porj

Architecture and implementation handoff for the Alpha Care Mental Health Workforce MVP.

This repository currently contains the project specification and coding-agent instructions. Application implementation has not started.

## Start here

- [Architecture and build roadmap](ARCHITECTURE_ROADMAP.md): product scope, architecture, database and API contracts, role permissions, 15 build milestones, 30 acceptance scenarios, and the verification ledger.
- [Agent instructions](AGENTS.md): how coding assistants should select work, consult requirements, test changes and record progress.

## Agreed stack

- React, TypeScript and Vite on Netlify.
- Node.js API and background worker on paid Render.
- Supabase PostgreSQL, Auth, private Storage and Queues.
- OpenRouter for AI APIs.

## Begin implementation

Open this repository in VS Code and start with milestone M00 in the roadmap. Inspect the current repository before selecting subsequent milestones. Use synthetic data during development and record passing test evidence before marking work verified.

Suggested coding-assistant prompt:

> Read AGENTS.md and ARCHITECTURE_ROADMAP.md. Inspect the repository and verification ledger, then implement the next eligible milestone. Run its required tests, record actual evidence, and update the ledger. Keep unresolved client policy decisions explicit and continue independent work where possible.
