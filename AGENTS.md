# Alpha Care project instructions

This companion belongs beside `ARCHITECTURE_ROADMAP.md` in the application repository root. If the project already has an `AGENTS.md`, merge these instructions with its existing instructions rather than overwrite it. Tools that do not automatically load `AGENTS.md` should be told to read both files in the initial prompt.

Before implementation:

1. Read `ARCHITECTURE_ROADMAP.md`, especially sections 1–4, the relevant workflow, the milestone in section 13 and the ledger in section 14.
2. Inspect current code and tests. Choose the next eligible milestone and record owner/branch/status; coordinate shared schema/contracts with colleagues.
3. Keep React on Netlify, Node.js API/worker on paid Render, Supabase for data/auth/private files/queues, and OpenRouter for AI.

During implementation:

- Build persistence, permissions, API, UI, failure handling and tests for each slice.
- Enforce the role matrix at database, API, file and export boundaries. Employees have no supervision access; hiring managers cannot manage training or read clinical notes/supervision.
- Preserve human approvals, exact document versions, once-per-occurrence credit, actual supervision attendance and a separate service-clearance decision.
- Use synthetic fixtures. Unresolved clinical/business policy follows section 15; keep affected production behavior disabled and continue independent work.
- Never mark mock-provider behavior as a live integration. Never weaken tests to turn a failure into a pass.

Before handoff:

- Run the milestone's applicable tests and record actual commands, results, tested commit and evidence in `docs/evidence/`.
- Update the roadmap ledger truthfully. Mark VERIFIED only when exit conditions pass; otherwise record IMPLEMENTED or BLOCKED and the missing work.
- Summarize changes, verification, blockers and the next eligible milestone. Update the specification when an approved contract changes.

For new projects/checkouts, use `D:\Codex` as the default parent unless Ankit specifies another location.
