# Activity Log

This log is append-only. Add new entries after all existing ones using `## [YYYY-MM-DD] <type> | <title>`. Prefer `ingest`, `query`, `decision`, `lint`, or `maintenance` as the type.

## [2026-09-04] maintenance | Organization repository initialized

Created the repository with a flat layout of `README.md`, `projects.md`, and a `decisions/` directory holding `DEC-001-repository-conventions`, `DEC-002-decision-placement`, and `DEC-003-public-identity`. Configured the repository-local Git identity `TENDER SYSTEMS`. No Wiki architecture, source layer, or schema existed at this point.

## [2026-09-05] maintenance | Aligned to the shared LLM Wiki architecture

Restructured the repository to the three-layer LLM Wiki convention already used by `other-goods-lab` and `longing-lab`: a `raw/` source layer, a `wiki/` synthesis layer, and an operating layer of `schema.md` and `AGENTS.md`.

`projects.md` was moved to `wiki/registry.md` and expanded into a system registry with identifiers, status, repositories, and descriptions. The three decision records moved from `decisions/` to `wiki/decisions/` unchanged. `decisions/README.md` was removed because its navigation role is fully carried by `wiki/index.md`; its content is preserved in Git history. `README.md` was rewritten so that the public-facing description stays intact and Wiki navigation is separated below it.

`AGENTS.md`, `schema.md`, `wiki/index.md`, `wiki/overview.md`, `wiki/current-state.md`, `wiki/log.md`, `raw/README.md`, and `raw/sources.md` were created. `raw/conversations/`, `raw/documents/`, `raw/surveys/`, and `raw/inbox/` were created empty. `wiki/concepts/`, `wiki/questions/`, and `wiki/systems/` were deliberately not created, because the schema forbids directories created before real material requires them.

No project knowledge was copied from either Lab repository. No raw source is registered yet. The institutional Git identity was verified rather than changed.
