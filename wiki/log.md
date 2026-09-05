# Activity Log

This log is append-only. Add new entries after all existing ones using `## [YYYY-MM-DD] <type> | <title>`. Prefer `ingest`, `query`, `decision`, `lint`, or `maintenance` as the type.

## [2026-09-04] maintenance | Organization repository initialized

Created the repository with a flat layout of `README.md`, `projects.md`, and a `decisions/` directory holding `DEC-001-repository-conventions`, `DEC-002-decision-placement`, and `DEC-003-public-identity`. Configured the repository-local Git identity `TENDER SYSTEMS`. No Wiki architecture, source layer, or schema existed at this point.

## [2026-09-05] maintenance | Aligned to the shared LLM Wiki architecture

Restructured the repository to the three-layer LLM Wiki convention already used by `other-goods-lab` and `longing-lab`: a `raw/` source layer, a `wiki/` synthesis layer, and an operating layer of `schema.md` and `AGENTS.md`.

`projects.md` was moved to `wiki/registry.md` and expanded into a system registry with identifiers, status, repositories, and descriptions. The three decision records moved from `decisions/` to `wiki/decisions/` unchanged. `decisions/README.md` was removed because its navigation role is fully carried by `wiki/index.md`; its content is preserved in Git history. `README.md` was rewritten so that the public-facing description stays intact and Wiki navigation is separated below it.

`AGENTS.md`, `schema.md`, `wiki/index.md`, `wiki/overview.md`, `wiki/current-state.md`, `wiki/log.md`, `raw/README.md`, and `raw/sources.md` were created. `raw/conversations/`, `raw/documents/`, `raw/surveys/`, and `raw/inbox/` were created empty. `wiki/concepts/`, `wiki/questions/`, and `wiki/systems/` were deliberately not created, because the schema forbids directories created before real material requires them.

No project knowledge was copied from either Lab repository. No raw source is registered yet. The institutional Git identity was verified rather than changed.

## [2026-09-05] ingest | Three institutional conversations registered

Registered `SRC-2026-09-04-apple-design-skill-review` (hash `6bf98420ba45c7f49ee13fbe25d001c714878a8c`), `SRC-2026-09-04-tender-systems-identity-review` (hash `d6e5cf6895846d41e684d9a55b2ec5b9d9a90df9`), and `SRC-2026-09-05-social-account-strategy` (hash `8a5a64971d40d8cb49a8ac2e5d911fb52d192424`) in `raw/sources.md`. The files arrived with exporter-generated names and were renamed to the `YYYY-MM-DD-short-slug.md` form required for registration; contents were not altered, and hashes were taken after renaming. All three are Korean-language conversation exports retained in their original language. These are the repository's first registered sources.

Promoted as confirmed: [[DEC-004-institutional-voice]] and [[DEC-005-public-facing-language]], both resting on statements the user made directly. [[DEC-003-public-identity]] was extended with public-surface rules the user supplied as established policy, without altering its original text.

Promoted as working or hypothesis: [[tender-duality]], [[public-surfaces]], and [[tender-subject-systematic-form]], the last recorded as `hypothesis` because the assistant named the pattern and the user did not confirm it.

Recorded as open: [[Q-001-shared-design-system]] and [[Q-002-internal-versus-public-language]].

Attribution care: the design-skill conversation ends with no user reply at all, so its layering model, its two English principles, and its proposed shared design skill are recorded as unconfirmed proposals rather than as direction. In the social-account conversation, the assistant's initial recommendation against per-system accounts and its stricter credential separation were both overridden by the user and are recorded as not adopted. The identity conversation's slogans, division names, and speculative subject-form pairings received no user response and were not promoted.

What was not copied: project-scoped material — per-system design observations, per-system public copy strings, and the product and index examples — was left in raw, with each Lab repository remaining canonical for it. The source files contain the operator's personal name; they are preserved unchanged as evidence, and the name was not carried into any Wiki page.

## [2026-09-05] ingest | Public release proposal registered

Registered [[SRC-2026-09-05-how-to-show]] at `raw/conversations/2026-09-05-how-to-show.md` with hash `a9fc7d974ce281c885da0c855e1348ca74374dd5`, preserving the supplied file unchanged. The excerpt contains assistant-voice recommendations without role labels or a user response; all promoted material remains `llm-proposed` and unconfirmed.

Extended [[public-surfaces]] with the proposed discovery-to-system route, web-first access, operational releases, gradual activation, and exhibition adaptation. This reinforces the existing public-language direction at proposal level without changing any decision. Extended [[Q-002-internal-versus-public-language]] with the unresolved tension between a proposed interpretive public archive and the existing public-copy rule. Updated [[current-state]] and [[index]]; no new page was needed.

Left candidate slogans, system-specific copy and implementation examples, illustrative rollout milestones, and external platform submission claims in raw. No Lab content was duplicated, no live platform facts were adopted, and no launch or archive was recorded as approved. All three previously registered source hashes matched before ingestion.
