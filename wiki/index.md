---
status: working
attribution: llm-synthesis
updated: 2026-09-05
sources: []
---

# TENDER SYSTEMS Wiki Index

This is the Wiki's working content catalog. Excluding the index itself, every Wiki page appears exactly once under its type using `link + one-line summary + status, when present + updated date`. Do not remove an entry unless its page is deleted. When a page's summary, status, or updated date changes, update this catalog in the same task.

## Routing

| Information to organize | Read or update first |
|---|---|
| Overall definition and operating principles of the institution | [[overview]] |
| Latest snapshot of institutional decisions, scope, and priorities | [[current-state]] |
| A system's identifier, status, repositories, or registry-level facts | [[registry]] |
| An idea that develops across several systems | Relevant `wiki/concepts/` page |
| A choice explicitly decided by the user and its rationale | Relevant `wiki/decisions/` page |
| An unanswered question that remains under review | Relevant `wiki/questions/` page |
| Chronological record of ingestion, queries, linting, and operational changes | Append to [[log]] |
| A new original and its hash or ingestion status | [Raw Source Index](../raw/sources.md) |
| Anything specific to one system's research, narrative, or creative direction | That system's Lab repository, not this one |

Before creating a page, check this catalog to see whether an existing page can be extended. Never classify `llm-proposed` material as a decision without explicit user confirmation.

## Core

- [[overview]] — Definition, operating principles, knowledge architecture, and public identity of TENDER SYSTEMS · `working` (2026-09-05)
- [[current-state]] — Snapshot of confirmed institutional decisions, current work, and unknowns · `working` (2026-09-05)
- [[registry]] — Canonical registry of systems operated by TENDER SYSTEMS, with identifiers, status, and repositories · `confirmed` (2026-09-05)

## Decisions

- [[DEC-001-repository-conventions]] — Repository roles, naming, and when each repository is created · `confirmed` (2026-09-04)
- [[DEC-002-decision-placement]] — Which repository a given decision belongs in · `confirmed` (2026-09-04)
- [[DEC-003-public-identity]] — The identity used on public-facing source control · `confirmed` (2026-09-04)

## Activity

- [[log]] — Append-only history of ingestion, queries, linting, decisions, and maintenance (2026-09-05)

## Repository Control

- [README](../README.md) — Public entry point for TENDER SYSTEMS and this repository; canonical English version (2026-09-05)
- [AGENTS](../AGENTS.md) — Reading, language, ingestion, cross-project boundary, public identity, institutional Git identity, and model-routing rules for agents (2026-09-05)
- [Schema](../schema.md) — Page taxonomy, status, attribution, provenance, file naming, scope boundary, and maintenance rules (2026-09-05)
- [Raw README](../raw/README.md) — How to add and preserve original source material, and what belongs in this repository's raw layer (2026-09-05)
- [Raw Source Index](../raw/sources.md) — IDs, paths, hashes, and ingestion status for every raw source (2026-09-05)

## Page Creation Gates

- Create `wiki/concepts/` and `wiki/questions/` only when registered material supports a real institution-level concept or open question. No such page exists yet.
- Create `wiki/systems/` only when a single system accumulates institution-level knowledge that develops independently of its Lab repository. Until then, [[registry]] holds every registry-level fact.
- Do not create a page for material that is canonical in a Lab repository. Link to that repository instead.
- Do not duplicate a per-source raw catalog here. Use the [Raw Source Index](../raw/sources.md) as the single registry.
