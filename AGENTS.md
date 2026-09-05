# TENDER SYSTEMS Wiki — Agent Instructions

This repository is TENDER SYSTEMS's long-term institutional memory. Agents working here read before they write. Before adding anything new, check what has already been recorded and build on it.

This repository defines the operating convention that `other-goods-lab` and `longing-lab` follow. When either diverges from this repository without reason, the convention recorded here governs.

## What to Read First

Read these files in order:

1. `wiki/index.md`
2. `wiki/current-state.md`
3. `wiki/registry.md`
4. `schema.md`
5. The concept, decision, or question pages relevant to the task

Do not begin by scanning the entire raw layer. Start with the synthesis already maintained in the Wiki, then consult only the raw sources that are necessary.

## Repository Language

- English is the canonical and default language for all maintained repository documentation, including `README.md`, `AGENTS.md`, `schema.md`, `wiki/**`, `raw/README.md`, and `raw/sources.md`.
- Write all new pages, edits, headings, summaries, metadata prose, and log entries in English, even when the user's working language is not English.
- Preserve proper names, source identifiers, file paths, code, and intentionally quoted source text when translating them would change their identity or evidentiary meaning. Add an English gloss when readers need one.
- Registered files under `raw/documents/`, `raw/conversations/`, and `raw/surveys/` are immutable source records and retain their original language. Never rewrite a raw source merely to satisfy the English-default policy; synthesize or explain it in English in the Wiki instead.
- Root `README.md` is the canonical English public entry point. Future public translations should use `README.<locale>.md` (for example, `README.ko.md`, `README.zh-CN.md`, and `README.ja.md`) and link back to the English original. Broader translated documentation may mirror canonical paths under `docs/i18n/<locale>/` when there is a real need.
- A translation is derivative, must be labeled with its locale and canonical English source, and must not introduce decisions or facts absent from the English original. When versions diverge, update English first and clearly mark any stale translation.

## Document Roles

- `README.md` is the entry point through which public readers understand TENDER SYSTEMS and this repository. Do not put the complete file list or agent instructions there.
- `wiki/index.md` is the working catalog for finding every Wiki page and its editing destination. Excluding the index itself, register each page exactly once under its type with `link + one-line summary + updated date`; include status when the page has one.
- `wiki/current-state.md` is a snapshot of currently valid decisions, scope, priorities, and unresolved questions.
- `wiki/registry.md` is the canonical registry of systems operated by TENDER SYSTEMS.
- `wiki/log.md` is an append-only chronological history of meaningful ingestion, queries, decisions, linting, and maintenance.
- `raw/sources.md` is the single registry for every original source's path, hash, and ingestion status. Do not duplicate the raw source list in the index.

## Query Workflow

When the user asks a question, find the answer in this order:

```text
index
  ↓
current-state
  ↓
registry
  ↓
relevant concept / decision / question
  ↓
raw source only when necessary
```

Consult raw sources only for consequential judgments or when the original evidence must be checked directly.

## Conversation Ingestion Workflow

When ingesting a new conversation or document, follow this sequence:

1. **Register the source** — Preserve the original unchanged under `raw/` and register it in `raw/sources.md` with its hash.
2. **Explore the existing Wiki** — Read the index, current state, and relevant pages first.
3. **Analyze the conversation** — Extract ideas, decisions, hypotheses, open questions, rejected or deferred ideas, rationale, tensions, and emerging concepts.
4. **Compare with existing knowledge** — Decide whether the information is new, reinforces existing material, conflicts with it, or supersedes an earlier decision.
5. **Decide whether to promote** — Keep the material only in raw or promote it into the Wiki.
6. **Prefer updating existing pages** — Before creating a page, check whether an existing page can be updated.
7. **Create a new page** — Do so only for a genuinely new, independent entity.
8. **Cross-link** — Link related concepts, decisions, and questions.
9. **Check current state** — Determine whether the organization's current state changed and update it when needed.
10. **Synchronize the index** — In the same task, update the catalog entry when a page is created, moved, or deleted, or when its summary, status, or updated date changes.
11. **Append to `log.md`** — Add the work after all existing entries using `## [YYYY-MM-DD] <type> | <title>`. Prefer `ingest`, `query`, `decision`, `lint`, or `maintenance` as the type.

## Cross-Project Knowledge Boundary

This repository is the institutional layer, not a project's memory. Detailed knowledge that belongs only to OTHER GOODS or LONGING stays canonical in that project's own Lab repository and is never copied here.

This repository stores only:

- Principles common to several systems.
- Institution-level decisions.
- The system registry.
- Cross-system relationships.
- Shared conventions.
- Shared research.
- Public identity.

When a claim about a specific system is needed here, link to the Lab repository that owns it rather than restating its content. Before recording anything, verify which repository is the canonical source for it; see [[DEC-002-decision-placement]].

## Never Do These Things

- Delete or modify a raw source.
- Replace raw material with the Wiki.
- Promote every source automatically.
- Record an LLM proposal as a user decision.
- Present a rejected idea as current.
- Invent facts without a source.
- Hide uncertainty.
- Silently overwrite older knowledge.
- Modify past entries in `log.md` outside an explicitly authorized repository-wide migration.
- Create many empty placeholder pages.
- Add metadata fields that are not needed.
- Treat Wiki size, page count, or document length as a success metric.
- Duplicate project-level knowledge from a Lab repository here.
- Expose the personal identity of the operator in repository content.

## When to Create a New Page

Create a page only when a meaningful unit has emerged that cannot be captured by one line in `current-state.md` and is likely to develop independently over time.

## Public Identity

The public-facing authorship of this organization's work is `TENDER SYSTEMS`. Write documents as institutional records, not as personal notes.

Do not use the operator's personal name, "my project," "I created," or any personal author attribution. Prefer institutional forms such as:

- "TENDER SYSTEMS defines ..."
- "The system currently operates ..."
- "This document records ..."

This governs new writing only. Do not rewrite existing Git history to remove personal identity. See [[DEC-003-public-identity]].

## Agent Model Routing Preference

For subagent model routing:

- Simple search and localization agents use the lightest available model tier.
- Document drafting and editing agents use the mid model tier.
- Planning and verification agents use the strongest available model tier.

## Git Identity and Push Policy

All Git commits created for this repository must use the institutional TENDER SYSTEMS identity rather than the personal identity of the operator.

### Commit identity

Before creating any commit, verify the repository-local Git identity.

Required identity:

- `user.name`: `TENDER SYSTEMS`
- `user.email`: `code@tender.systems`

This institutional email is already established and verified for this organization; see [[DEC-003-public-identity]]. Use repository-local configuration:

```bash
git config --local user.name "TENDER SYSTEMS"
git config --local user.email "code@tender.systems"
```

Do not modify the operator's global Git identity unless explicitly requested. Never fall back to the operator's personal name or personal email address.

Even though the institutional email for this organization is established, an agent must never invent or guess an institutional email in a repository where it has not been verified. If the applicable TENDER SYSTEMS email cannot be verified from the existing environment, DEC-003, or GitHub configuration, do not invent one and do not use a personal email address. In particular, do not guess a Gmail address, a `tendersystems` domain address, or a `noreply` address. Stop before committing and report that the institutional email must be configured.

Before every commit, verify:

```bash
git var GIT_AUTHOR_IDENT
git var GIT_COMMITTER_IDENT
```

Both identities must resolve to the TENDER SYSTEMS institutional identity.

After creating a commit, verify with:

```bash
git log -1 --format=fuller
```

The author and committer must not contain the operator's personal identity.

### Push authentication

Commit identity and GitHub push authentication are separate concerns. Setting `git config user.name` or `user.email` does not determine which GitHub account performs the push.

Before pushing, identify which GitHub account or automation identity will authenticate the operation. A dedicated institutional identity remains preferred. Acceptable institutional mechanisms include:

- a dedicated TENDER SYSTEMS GitHub user or machine account with its own SSH key;
- a dedicated TENDER SYSTEMS GitHub credential or token;
- a GitHub App or another explicitly configured institutional automation identity.

Do not assume that membership in the `TENDER-SYSTEMS-LAB` GitHub Organization makes the Organization itself a Git authentication identity.

The public commit history derives author and committer attribution from the commit object, not from the account that authenticated a later push. When the user explicitly authorizes personal push authentication on that basis, the agent may use it only after confirming that the public commit record contains the institutional author and committer identity. Do not describe personal authentication as institutional authentication, and do not promise that the push actor is anonymous: GitHub organization audit logs or other non-commit activity surfaces may retain the authenticating account.

#### Standing authorization for this repository

On 2026-09-05, the user explicitly authorized using the operator's personal GitHub authentication to push this repository, acknowledging that the push actor may remain visible in GitHub audit logs or other non-commit activity surfaces. This authorization persists for subsequent requested pushes to `TENDER-SYSTEMS-LAB/tender-systems`; do not ask for the same approval again unless the authorization is revoked or the task explicitly requires a dedicated institutional push identity.

Before each push, still verify the actual authentication identity and confirm that every outgoing commit has `TENDER SYSTEMS <code@tender.systems>` as both author and committer. This permission does not authorize personal commit attribution, disclosure of personal identity in repository content, or pushes that were not otherwise requested. It does not grant standing authorization for other repositories.

If a dedicated TENDER SYSTEMS push identity is required for the task, do not fall back to the operator's personal credentials.

Where SSH is used, prefer a dedicated SSH host alias and key configuration that isolates TENDER SYSTEMS authentication from the operator's personal GitHub identity. Where HTTPS is used, keep TENDER SYSTEMS credentials isolated from personal GitHub credentials.

Never expose, print, commit, or document secrets such as:

- personal access tokens;
- OAuth tokens;
- private SSH keys;
- credential-helper secrets.

### Pre-commit and pre-push safety rule

Before any `git commit`, the agent must verify:

1. The repository is a TENDER SYSTEMS repository.
2. `user.name` resolves to `TENDER SYSTEMS`.
3. `user.email` resolves to the verified TENDER SYSTEMS email.
4. The author and committer identities do not contain the operator's personal identity.

Before any `git push`, the agent must additionally verify the actual authentication identity. Use a dedicated TENDER SYSTEMS identity unless the user has explicitly authorized personal push authentication after being informed that the actor may remain available in audit logs or other non-commit activity surfaces. The standing authorization above satisfies the personal-authentication approval requirement for this repository. In either case, verify that the commits being pushed retain the institutional author and committer identity.

If the applicable conditions cannot be verified, do not commit or push. Report the unresolved configuration instead.

### Existing history

Do not rewrite existing Git history merely because older commits contain a personal identity. Unless explicitly instructed otherwise, do not use:

- `git filter-repo`;
- history-rewriting rebase operations;
- force push;
- author rewriting of existing commits.

This policy applies to new commits from this point forward.

## Verification

At the beginning and end of a task, verify that source originals have not changed since registration:

```bash
git hash-object raw/documents/*.md raw/conversations/*.md raw/surveys/*.md
```

Compare the results with the `Hash` column in `raw/sources.md`. If any value differs, the original changed. Do not update the Wiki automatically; mark the relevant page `REVIEW_REQUIRED`.
