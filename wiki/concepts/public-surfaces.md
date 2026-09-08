---
status: working
attribution: jointly-developed
updated: 2026-09-08
sources:
  - SRC-2026-09-05-how-to-show
  - SRC-2026-09-05-social-account-strategy
  - SRC-2026-09-08-youtube-content-plan
---

# Public Surfaces

How the institution appears on public platforms outside source control.

## Current state

On 2026-09-05 the user reported that Instagram and YouTube accounts had been created, confirming it directly:

> "오케이 인스타 유튜브 다 만들었어."

Three entities each hold their own account on both platforms: the institution (`TENDER SYSTEMS`), OG-001 (`OTHER GOODS`), and LN-001 (`LONGING`).

The exact live handles are **not verified**. The user's own message in the conversation shows the intended Instagram set:

```text
TENDER SYSTEMS
@tendersystems

OTHER GOODS
@othergoods.og001

LONGING
@longing.ln001
```

The user then reported that the first of these was already taken:

> "이렇게 만드려고 했는데, 'tendersystems' 이게 이미 있대"

after which the assistant recommended `@tender.systems` as the replacement for the institutional handle. The user never restated the final strings used at account creation. All three Instagram handles are therefore marked `unknown` and need verification against the live accounts.

The same applies to YouTube. The user rejected the platform-generated fallback handle for LONGING, `LONGING-m1u`, and the assistant proposed alternatives (`@LONGING-LN001` recommended first, among others). The chosen handle is not recorded in the conversation and is likewise `unknown`.

## Account structure

The institution operates one account per entity rather than a single institutional account covering all three. The assistant's first recommendation in the conversation was against separate per-system accounts, favoring a single `TENDER SYSTEMS` account with the individual systems appearing inside it as internal sections. The user's next message overrode this, proposing the split directly:

> "Instagram 계정도 TENDER SYSTEMS와 OTHER GOODS, LONGING 을 각각 만들어보면 어때?"

The split was settled by the user creating the accounts (see Current state above), not by the assistant's initial recommendation.

## Handle grammar

The institutional handle carries no system code. A per-system handle appends its system code (`og001`, `ln001`) to the system name. The separator differs by platform in the conversation's examples: dot-separated on Instagram (`othergoods.og001`, `longing.ln001`) and hyphenated on YouTube (`OTHERGOODS-OG001`, `LONGING-LN001`).

Display names stay bare — `TENDER SYSTEMS`, `OTHER GOODS`, `LONGING` — with no code appended, and the system codes appear in the bio rather than in the display name.

This grammar was proposed by the assistant. It was adopted by the user through use — by acting on it when creating accounts — rather than by an explicit confirming statement in the conversation. The platform-by-platform separator difference (dot on Instagram, hyphen on YouTube) is the assistant's own recommendation, not a rule the user stated.

## Voice

Each system's account is written as the system operating, not as an account describing the system — for example, OTHER GOODS's account speaks as a store rather than as a page about an artwork. Per-system copy does not announce the parent institution; the shared identifier pattern (system name plus system code) across accounts is what lets the accounts read as one institution without stating it. See [[DEC-005-public-facing-language]].

Per-system bio strings are maintained in each system's own Lab repository and are not recorded on this page.

## Management

The accounts are managed from the operator's existing personal application session, using its add-account facility, rather than through fully separated institutional credentials. The assistant first recommended stricter separation — credentials and recovery email owned by the institution rather than the personal account, to ease future handoff and to keep the personal account structurally outside the institution's account tree. The user then proposed the simpler arrangement, citing solo management:

> "나는 아예 개인계정에서 그냥 계정 추가를 하는 방법을 생각 했는데 이건 별로인가?"

The assistant revised its recommendation in response, judging the stricter separation unnecessary for a single, ongoing solo operator and endorsing the add-account approach instead. The adopted approach is user-originated; the assistant's earlier stricter proposal was not adopted. The security measures the assistant listed alongside the revised recommendation — separate passwords per account, app-based 2FA, recovery email routed to an institutional address, contact-sync disabled — were not confirmed by the user in the conversation.

## Unresolved

Which platform comes next is undecided. The assistant proposed a sequence — Threads, then X, then Bluesky, then TikTok — but the conversation ends before any user reply to this proposal. This ordering is `llm-proposed` and unconfirmed.

Platform facts cited by the assistant in that exchange — a Threads monthly-active-user figure and X's username length limit — came from assistant web searches conducted on 2026-09-05 and need re-verification before use, since they were not independently checked against a registered source.

A fourth public surface has since been proposed: a video channel voiced by the operator in the first person, distinct from the three entity accounts recorded above. No channel was created, and no name was adopted; the plan's episode list, ordering, video structure, and proposed name are `llm-proposed` and received no user reply. The user's own contribution is four seed topics, two derived topic titles, and a preference for a weekly cadence:

> "한주에 하나씩 영상을 공개하면 좋을 것 같네."

Whether such a surface is permitted, and under whose identity it would run, is open — see [[Q-003-operator-voice-on-public-channels]].

## Proposed release and discovery structure

Status: `hypothesis`; attribution: `llm-proposed`.

The how-to-show excerpt proposes extending the existing operating voice into the audience's route through the work: social discovery or a minimal institutional index leads directly to an independently accessible system website, with archive and research material in a separate layer. Instagram and YouTube would function as discovery surfaces speaking in the systems' operating registers, while GitHub would support documentation rather than serve as the audience's first entrance.

The proposal favors web access without installation, reserving native apps for work whose material depends on device capabilities. It also suggests releases presented as systems becoming operational, gradual activation and expansion rather than one complete launch, and physical exhibitions that adapt a system's operations to a space. These are options for cross-system presentation, not an approved release plan, implementation choice, or exhibition commitment.

This reinforces the language principle in [[DEC-005-public-facing-language]] at proposal level and extends it to distribution. A separate public archive containing interpretive writing raises an unresolved boundary with that principle; see [[Q-002-internal-versus-public-language]]. No website, archive, launch sequence, or additional platform is confirmed by this excerpt. Specific system copy, interface and exhibition examples, candidate slogans, and external submission recommendations remain in raw; the Lab repositories in [[registry]] remain canonical for system-specific choices.

The excerpt has no user reply and is the sole source for this release structure. Its external platform references have not been independently verified.

## Related

- [[DEC-003-public-identity]]
- [[DEC-005-public-facing-language]]
- [[registry]]

## Sources

- [[SRC-2026-09-05-how-to-show]] — [raw/conversations/2026-09-05-how-to-show.md](../../raw/conversations/2026-09-05-how-to-show.md)

- [[SRC-2026-09-05-social-account-strategy]] — [raw/conversations/2026-09-05-social-account-strategy.md](../../raw/conversations/2026-09-05-social-account-strategy.md)

- [[SRC-2026-09-08-youtube-content-plan]] — [raw/conversations/2026-09-08-youtube-content-plan.md](../../raw/conversations/2026-09-08-youtube-content-plan.md)

The assistant used live web search during this conversation and cited external help-centre and newsroom pages (Instagram/Meta Help Centre, X Help, a Meta newsroom post) that are not registered as sources in this repository; treat facts drawn from them as unverified until a source is registered. The assistant's account of LONGING's own Wiki, consulted while drafting bio copy, is a secondary citation here — the primary material lives in longing-lab, which remains canonical.
