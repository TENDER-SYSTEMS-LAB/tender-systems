---
status: working
attribution: llm-synthesis
updated: 2026-09-09
sources:
  - SRC-2026-09-08-youtube-visual-identity
  - SRC-2026-09-08-bibliography-survey
  - SRC-2026-09-08-human-social-engineering-models
  - SRC-2026-09-08-youtube-content-plan
  - SRC-2026-09-07-chatgpt-artist-name-survey
  - SRC-2026-09-07-claude-artist-name-survey
  - SRC-2026-09-07-deepseek-artist-name-survey
  - SRC-2026-09-07-gemini-artist-name-survey
  - SRC-2026-09-07-glm-artist-name-survey
  - SRC-2026-09-07-grok-artist-name-survey
  - SRC-2026-09-07-qwen-artist-name-survey
  - SRC-2026-09-07-academic-guidance-and-leonardo-publication
  - SRC-2026-09-05-how-to-show
  - SRC-2026-09-04-apple-design-skill-review
  - SRC-2026-09-04-tender-systems-identity-review
  - SRC-2026-09-05-social-account-strategy
  - SRC-2026-09-06-creative-origin-and-motivation
  - SRC-2026-09-06-engineering-background-and-artistic-possibility
  - SRC-2026-09-06-traceable-creative-process
  - SRC-2026-09-07-creator-motivation-statements
  - SRC-2026-09-07-alganzi-ai-video
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
| Inspiration, motivation, or reflection shared across works and retained as background memory | Relevant `wiki/notes/` page |
| A choice explicitly decided by the user and its rationale | Relevant `wiki/decisions/` page |
| An unanswered question that remains under review | Relevant `wiki/questions/` page |
| Chronological record of ingestion, queries, linting, and operational changes | Append to [[log]] |
| A new original and its hash or ingestion status | [Raw Source Index](../raw/sources.md) |
| Anything specific to one system's research, narrative, or creative direction | That system's Lab repository, not this one |

Before creating a page, check this catalog to see whether an existing page can be extended. Never classify `llm-proposed` material as a decision without explicit user confirmation.

## Core

- [[overview]] — Definition, operating principles, knowledge architecture, and public identity of TENDER SYSTEMS · `working` (2026-09-07)
- [[current-state]] — Snapshot of confirmed institutional decisions, current work, background records, and unknowns · `working` (2026-09-09)
- [[registry]] — Canonical registry of OG-001, LN-001, and RS-001, with status and repositories · `confirmed` (2026-09-07)

## Concepts

- [[tender-duality]] — The two senses of `tender`, tenderness and transaction, that the institution works between · `working` (2026-09-07)
- [[tender-subject-systematic-form]] — Proposed structural method shared by the current systems, unconfirmed, with proposed supporting literature · `hypothesis` (2026-09-08)
- [[public-surfaces]] — Accounts, handles, voice, management, an unconfirmed release and discovery structure, and an operator-channel working visual direction · `working` (2026-09-09)

## Notes

- [[artist-name-survey]] — Seven LLM artist-name recommendations, competing interpretations, and verification limits; no personal name adopted · `working` (2026-09-07)

- [[academic-guidance-and-publication]] — Interest in academic guidance, 강이연 and Leonardo, with unconfirmed candidates and preparation routes · `working` (2026-09-07)

- [[creative-origin-and-motivation]] — AI enjoyment, engineering background, artistic possibility, process traceability, and three stated motivations on disappearing romance, self-funded practice, and trust, love, and understanding; background memory, not an adopted philosophy · `working` (2026-09-07)

- [[bibliography-survey]] — Unadopted reference survey: institution-level artworks and papers, an annotated bibliography document, and two proposed reading disciplines · `working` (2026-09-08)

## Decisions

- [[DEC-001-repository-conventions]] — Repository roles, naming, and when each repository is created · `confirmed` (2026-09-04)
- [[DEC-002-decision-placement]] — Which repository a given decision belongs in · `confirmed` (2026-09-04)
- [[DEC-003-public-identity]] — The identity used on public-facing source control, extended with public-surface rules and a closed exception for registered originals · `confirmed` (2026-09-08)
- [[DEC-004-institutional-voice]] — Presents as an organization, reads as one brand, derived from the systems already built · `confirmed` (2026-09-07)
- [[DEC-005-public-facing-language]] — Public copy states what a system does and never explains or labels the work · `confirmed` (2026-09-07)

## Open Questions

- [[Q-001-shared-design-system]] — Whether one design discipline should govern every system, and what governs what · `unknown` (2026-09-07)
- [[Q-002-internal-versus-public-language]] — Boundaries of internal language and a proposed public interpretive archive · `unknown` (2026-09-07)
- [[Q-003-operator-voice-on-public-channels]] — Whether operator-voiced explanatory video falls under the public-language rule, and under whose identity such a channel would run · `unknown` (2026-09-09)

## Activity

- [[log]] — Append-only history of ingestion, queries, linting, decisions, and maintenance (2026-09-09)

## Repository Control

- [README](../README.md) — Concise public entry point with the institutional tagline, system links, overview, and archive (2026-09-07)
- [AGENTS](../AGENTS.md) — Task-sized reading, scoped verification, source preservation, institutional Git identity, and standing push authorization (2026-09-07)
- [Schema](../schema.md) — On-demand page structure, attribution, provenance, catalog, and maintenance reference (2026-09-07)
- [Raw README](../raw/README.md) — New-source registration, immutable originals, and targeted lookup guidance (2026-09-07)
- [Raw Source Index](../raw/sources.md) — Source IDs, paths, hashes, ingestion status, and targeted registration/lookup rules (2026-09-08)

## Page Creation Gates

- Create `wiki/systems/` only when a single system accumulates institution-level knowledge that develops independently of its Lab repository. Until then, [[registry]] holds every registry-level fact.
- Keep the choice of the next public platform in [[public-surfaces]] rather than opening a page for it.
- Create a design page only if [[Q-001-shared-design-system]] receives a user decision. The material on record is an unanswered proposal.
- Do not create a page for material that is canonical in a Lab repository. Link to that repository instead.
- Do not duplicate a per-source raw catalog here. Use the [Raw Source Index](../raw/sources.md) as the single registry.
