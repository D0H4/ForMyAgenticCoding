## Repository Knowledge Harness

This repository uses a canonical documentation layer for repository knowledge.

Canonical repository guidance lives in `canonical_docs/`.

Agents must not read all canonical documents by default.

Agents must begin by reading:
- `canonical_docs/REPO_MAP.md`
- `canonical_docs/TASKS.md`
- `canonical_docs/STYLEGUIDE.md`

Agents must then read only the additional canonical documents required for the current task.

Additional canonical document routing rules:

- Read `ARCHITECTURE.md` for architecture, dependency, boundary, module ownership, or data-flow changes.
- Read `TESTING.md` for any test-writing, test-editing, test-running, coverage, or validation task.
- Read `WORKFLOW.md` for build, run, lint, format, CI, release, or development workflow tasks.
- Read `FRONTEND_GUIDE.md` for frontend UI implementation, component design, styling, layout, interaction, accessibility, responsive behavior, or design-system-related tasks.

If a task spans multiple areas, read all relevant canonical documents for those areas.

Canonical documentation is the authoritative source for repository behavior.
Legacy documentation may be used only for reference.
If canonical documentation conflicts with legacy documentation, canonical documentation takes precedence.

# Rules
- NEVER READ .env FILE.
- DO NOT EDIT `AGENTS.md`, `CLAUDE.md`, `GEMINI.md` FILE.
- DO NOT USE SUBAGENTS FEATURE.
