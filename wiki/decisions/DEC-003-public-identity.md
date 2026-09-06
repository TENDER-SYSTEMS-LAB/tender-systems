---
status: confirmed
attribution: user-confirmed
updated: 2026-09-07
sources:
  - SRC-2026-09-04-tender-systems-identity-review
---

# DEC-003 — Public Identity

## Decision

Source control under this organization uses one identity:

```text
TENDER SYSTEMS <code@tender.systems>
```

It is configured per repository, never globally:

```bash
git config --local user.name "TENDER SYSTEMS"
git config --local user.email "code@tender.systems"
```

Before the first commit in any repository, verify that both the author and the committer resolve to this identity:

```bash
git var GIT_AUTHOR_IDENT
git var GIT_COMMITTER_IDENT
```

The account used to authenticate with the hosting provider is administrative infrastructure. It is not the public identity of the work, and it is not used as a commit identity.

## Rationale

Authentication and attribution are different things. A repository's public record should carry the identity of the practice, not of whoever happened to be at the keyboard.

## Consequences

- Global Git configuration is never modified to achieve this; a repository-local setting is used.
- Commits carry no `Co-authored-by`, `Signed-off-by`, or tool-attribution trailers.
- Commit messages describe the change and nothing else.
- Repository metadata — descriptions, topics, profile text — carries no personal attribution, biography, or contact details.

## Extension (2026-09-05)

A registered source — an operational instruction the user pasted for GitHub Organization profile and repository metadata cleanup — reaffirmed this decision and added public-surface rules stated by the user as established policy:

- The public identity is unified as `TENDER SYSTEMS`.

  > "공개 identity는 `TENDER SYSTEMS`로 통일한다."

- The operator's personal identity is not exposed on public surfaces. (The source states this rule by naming the operator directly; that name is omitted here and the quote is not reproduced because it contains a personal name.)

- GitHub Organization membership stays private.

  > "Organization membership은 Private 상태를 유지한다."

- Repository Topics are empty for the current repositories; technical topics may be considered later only for a genuine public software repository, and only for that repository.

- The organization profile README stays minimal: name, one line, the active systems, nothing further.

- The public listing uses the heading `ACTIVE SYSTEMS` rather than a projects or works heading.

  > "ACTIVE PROJECTS가 아니라 ACTIVE SYSTEMS를 사용하는 것도 중요한 선택이다."

- Commit author and committer remain `TENDER SYSTEMS <code@tender.systems>`, configured locally, never globally.

These were presented in the source as already-established policy rather than decided in that conversation.

- See [[DEC-004-institutional-voice]] and [[DEC-005-public-facing-language]].

## Sources

- [[SRC-2026-09-04-tender-systems-identity-review]] — [raw/conversations/2026-09-04-tender-systems-identity-review.md](../../raw/conversations/2026-09-04-tender-systems-identity-review.md)

The source is a conversation export in which these rules appear inside a user-pasted instruction block.
