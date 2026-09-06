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

## [2026-09-05] maintenance | Recorded standing push authentication authorization

The user explicitly authorized personal GitHub authentication for this repository after being informed that the push actor may remain visible in audit logs or other non-commit activity surfaces, and requested that `AGENTS.md` record the permission. Updated the policy to preserve this authorization for subsequent requested pushes to this repository without repeated approval. Every outgoing commit must still use the institutional author and committer identity, and authentication must still be verified before each push. The permission does not extend to other repositories or authorize unsolicited pushes. Updated the control-document catalog entry in [[index]]. No personal account identifier or credential was recorded.

## [2026-09-06] ingest | Creative origin and motivation preserved as background

Registered [[SRC-2026-09-06-creative-origin-and-motivation]] with hash `8ba347366ddac7087d51351ec4e7c18757b2306f`, preserving the user's complete Korean message, including its literal HTML space entities. All four previously registered source hashes matched before ingestion.

Created [[creative-origin-and-motivation]] as a `user-originated` background note for later recollection of how the work began. Preserved the comparison between spending on books, performances, play, and travel and the apparent lack of shared noncommercial AI experiences, the enjoyment behind the question, and the gradual development of this initial inspiration and continuing motivation. Observations about other people's behavior remain a personal impression, not a verified finding. No philosophy, institutional principle, or public statement was adopted.

Added the `note` page type and its naming and scope guidance to `schema.md` for this actual material. Registered the page under Notes in [[index]] and linked it separately under Background records in [[current-state]]. Existing decisions and public-language questions remain unchanged. No project-specific knowledge was copied from a Lab repository.

## [2026-09-06] ingest | Engineering background and artistic possibility added to the origin note

Registered [[SRC-2026-09-06-engineering-background-and-artistic-possibility]] with hash `a3b0a4b17bd6a03e050213c11225127ea52c428b`, preserving the complete Korean follow-up unchanged. All five previously registered source hashes matched before ingestion.

Extended [[creative-origin-and-motivation]] with a dated Evolution section covering the self-described computer science/engineering and software-development background, DevOps work, identification with advanced LLM use, and the possibility that spending tokens and money on conceptual art could interest others and enable artistic self-realization. Audience interest or demand remains a question, and the apparent rarity of similar practice remains a personal impression. This supplements the earlier enjoyment and curiosity without adopting a philosophy or commercial objective. Updated [[index]], [[current-state]], and the note's provenance to include both direct accounts.

## [2026-09-06] ingest | Traceable creative process added to the origin note

Registered [[SRC-2026-09-06-traceable-creative-process]] with hash `966aae81af1b86ee342692ac1dbfe522ad1eec88`, preserving the complete Korean follow-up unchanged. All six previously registered source hashes matched before ingestion.

Extended [[creative-origin-and-motivation]] with a dated reflection on using GitHub and a Wiki to retain work records, AI conversations, and decision-making so that the creative process can be retraced. Preserved the user's thought that this recording practice could itself be an interesting feature of the work's world, without treating it as an adopted philosophy, a confirmed artwork boundary, or proof of complete archival coverage. Shortened the page heading to encompass the accumulated reflections and synchronized its catalog summary, background entry, and source references in [[index]] and [[current-state]].


## [2026-09-06] lint | Link source files from every Sources entry

- `## Sources` entries named each original as plain text, so a page's provenance was readable but not navigable and the raw files reached the graph only through `raw/sources.md`. Rewrote 27 entries across 10 pages as `[[SRC-...]] — [raw/<type>/<file>.md](<relative path>)`, keeping the wikilink as the shared source identifier and adding the file itself as a Markdown link.
- `schema.md`: the Provenance example now shows both links and states the relative-path rule — `../raw/...` from a page directly under `wiki/`, `../../raw/...` from a page in a subdirectory.
- No claim, attribution, status, or hash changed. This is a link-format correction only.

## [2026-09-06] lint | Re-register the traceable creative process source

- `raw/sources.md` held no row for `SRC-2026-09-06-traceable-creative-process`, while the log entry above, the origin note, current state, and the index all cite it. The file was present but untracked.
- Restored the registry row and its capture note. The file hashes to `966aae81af1b86ee342692ac1dbfe522ad1eec88`, matching the value the earlier entry recorded, so the original is unchanged and no dependent page needs `REVIEW_REQUIRED`.
- Registering a source and committing it are separate steps. Commit `raw/conversations/2026-09-06-traceable-creative-process.md` together with this registry row; until then the row points at a file the repository does not track.

## [2026-09-07] maintenance | Verify the pending documentation handoff

Reviewed the pending source-link maintenance and traceable-creative-process ingestion. The new source hash matches its registry row; previously tracked originals have no changes under `raw/`. The creative-process reflection remains background memory, with no promotion to a user decision or institutional principle.

Synchronized the 11 changed content pages and their catalog dates, the index metadata, and the activity and schema entries. Every Wiki page remains cataloged once with its existing status, and the changed pages' local source links resolve. The earlier source-link lint entry overstates its count: the reviewed diff converts 19 existing plain-text source paths across 10 pages, not 27. The new source references belong to the separate ingestion change. Existing log entries are preserved unchanged.
