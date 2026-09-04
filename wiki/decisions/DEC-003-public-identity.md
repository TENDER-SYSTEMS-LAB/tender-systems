---
status: confirmed
attribution: user-confirmed
updated: 2026-09-04
sources: []
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
