---
status: confirmed
attribution: user-confirmed
updated: 2026-09-09
sources:
  - SRC-2026-09-09-operator-channel-boundary
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

## Extension (2026-09-08) — registered originals

Some registered originals under `raw/` contain the operator's personal name, because the conversations they preserve mention it. On 2026-09-08 the user decided that this is not to be remediated: the affected originals stay published unchanged and the matter is closed.

The rule itself is unchanged and applies to everything the institution writes. Maintained documentation — Wiki pages, the README, the registry, repository metadata, commit identity — carries no personal attribution. Raw originals are evidence and are never edited, so the exception is a property of the evidence layer, not a relaxation of the rule.

Do not raise this again as an open issue, and do not rewrite history, redact a registered original, or register a masked replacement on account of it.

## Evolution (2026-09-09) — operator-channel boundary

The earlier broad public-surface wording left operator-voiced commentary unresolved. The user now confirms a distinct communicative surface: the operator channel does not identify its speaker as the maker of TENDER SYSTEMS or present itself as the institution's official behind-the-scenes channel. It may refer indirectly and approximately to making work, in the maker's own voice, without displaying or explaining the institutional identity principles.

This defines the channel's voluntary disclosure, not a requirement for absolute anonymity or for preventing an audience from inferring a connection. It does not establish a channel name, live account, or account ownership. Institutional and system surfaces retain their existing identity rules; maintained institutional records and Git attribution are unchanged. See [[DEC-005-public-facing-language]] and the resolution in [[Q-003-operator-voice-on-public-channels]].

## Sources

- [[SRC-2026-09-09-operator-channel-boundary]] — [raw/conversations/2026-09-09-operator-channel-boundary.md](../../raw/conversations/2026-09-09-operator-channel-boundary.md)

- [[SRC-2026-09-04-tender-systems-identity-review]] — [raw/conversations/2026-09-04-tender-systems-identity-review.md](../../raw/conversations/2026-09-04-tender-systems-identity-review.md)

The source is a conversation export in which these rules appear inside a user-pasted instruction block.
