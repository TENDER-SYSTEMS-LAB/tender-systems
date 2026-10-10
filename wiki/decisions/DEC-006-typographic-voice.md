---
status: confirmed
attribution: user-confirmed
updated: 2026-10-10
sources:
  - SRC-2026-09-14-typographic-voice
  - SRC-2026-10-10-typeface-as-persona
---

# DEC-006 — Typeface Identifies the Speaker

## Decision

Across TENDER SYSTEMS and the systems it operates, typeface distinguishes **who is speaking**, not what kind of content is being shown. A heading, a caption, and a body paragraph do not automatically differ; a machine reading, a system record, and a human interpretation do.

The user stated the rule directly:

> "누가 말하고 있는가에 따라 서체가 달라지는 것이 중요한것 같아.
> 시스템이 만들어내고 말하는 글꼴과 사람이 쓴글을 달라야해."

Three assignments carry it:

| Speaker | Typeface | Where it appears |
|---|---|---|
| The system | Inconsolata | Prices, dates, codes, status values, metadata, general interface text, system-generated sentences |
| The machine, more directly | Departure Mono | Terminals, dashboards, monitoring surfaces, logs, live status |
| A person | Source Serif | Analyst reports, essays, interpretation, commentary — long text a human wrote |

Inconsolata is the base typeface. Departure Mono was considered as a replacement for it and deliberately was not adopted as one; it carries the narrower role above, where the user wants a surface to read as more mechanical than Inconsolata makes it.

## Why typeface matters

On 2026-10-10 the user stated the reason behind the rule, and directed that it be reflected in the works:

> "글꼴이 중요한 이유는 글이 말 그 자체라면 글꼴은 말투나 말하는 화자에 대한 페르소나 이기 때문이라고 생각한다.
> 이 철학이 작품들에게 반영되어야 한다."

If the text is the speech itself, the typeface is how it is spoken and who is heard speaking it. This is the `user-originated` ground of the decision. It explains why the speaker, rather than the content type, selects the typeface. The rest of this paragraph is `llm-synthesis`, not the user's words. It also means a typeface is chosen for the persona it gives a voice, and not only to mark which voice is which. The three families above are the current casting of three personas. If a family is replaced, its successor must carry the same persona, not just stay visually distinct.

## Why this is institutional

The rule applies to more than one system, and it survives a rebuild of any of them, which is the test in [[DEC-002-decision-placement]]. It also outlives its own implementation: the three typefaces may be replaced, while the reason for distinguishing the speakers remains. Each system's own application of the rule — density, hierarchy, screen layout — stays canonical in that system's Lab repository.

## How it was reached

**Evolution.** The user opened with a reference image and asked for a work-wide typeface with the feel of one used for code. The assistant proposed IBM Plex Mono and a per-system split between Sans and Mono. The user then added a concrete requirement:

> "숫자 0을 쓸 때 가운데 사선으로 "/"가 쳐져 있으면 좋겠어"

That requirement set IBM Plex Mono aside. Of the candidates offered — Inconsolata, Anonymous Pro, JetBrains Mono Slashed, Input Mono — the user chose the first:

> "Inconsolata 으로 결정 하면 좋을 것 같아."

The user then raised Departure Mono. The assistant recommended keeping Inconsolata and giving Departure Mono a separate display role. Separately, the user asked for a different typeface for research reports, because a person writes them, and accepted the proposal:

> "Source Serif 좋은것 같아."

and extended Departure Mono's role themselves:

> "터미널 대시보드와 같은건 Inconsolata보다 더 기계스럽게 Departure Mono를 사용하도록 하고 싶어."

On 2026-10-10 the user added the rationale recorded under *Why typeface matters*. This **reinforces** the rule rather than revising it: no assignment changed.

The earlier direction — one Sans/Mono split assigned per system — is superseded by this one. It was never adopted, so it is not recorded as rejected material elsewhere.

## What is not settled

- **Korean text.** The assistant recommended against setting long Korean text in a monospace face and left the auxiliary Korean sans unnamed. An early suggestion of IBM Plex Sans KR belongs to the superseded IBM Plex direction. No Korean typeface is decided.
- **Version and weights.** The user said "Source Serif"; "Source Serif 4" is the assistant's specification. Weight, size, spacing, and hierarchy suggestions — Regular with Medium where needed, hierarchy from size and whitespace rather than weight — are `llm-proposed`.
- **Per-system density.** A table assigning each of the four systems a characteristic density and impression is `llm-proposed`, as is the English formulation "Typography identifies the speaker." The rule of record is the user's Korean statement above.
- **The reference.** The typeface in the user's reference image is never identified, and the image binaries are remote links absent from the export.
- **Glyph and licensing claims.** Which families carry a slashed zero by default, and the licensing statements about each candidate, are the source assistant's reports and were not verified during ingestion. Verify before implementation.

- **Tone versus speaker.** The user's rationale names both *말투* (manner of speech) and the speaker's persona. Whether a change of manner within one speaker — a dry record and a warm description, both issued by the same system — should ever change the typeface is not stated. Until the user says otherwise, the speaker remains the only thing that selects a typeface. OTHER GOODS records a local reading that treats register as separate from speaker. That reading is `llm-proposed`.

## Scope boundary

This decision governs the institution and its systems. It does not change the operator channel's working visual direction in [[public-surfaces]], which is a deliberately separate surface with its own recorded typography.

## Related

- [[design-principles]] — the abstract layer this decision is an instance of; its fourth principle, that form follows role, is the same idea stated more generally
- [[Q-001-shared-design-system]] — the open question about shared design discipline, which this partially answers
- [[DEC-002-decision-placement]]
- [[current-state]]

## Sources

- [[SRC-2026-09-14-typographic-voice]] — [raw/conversations/2026-09-14-typographic-voice.md](../../raw/conversations/2026-09-14-typographic-voice.md)

- [[SRC-2026-10-10-typeface-as-persona]] — [raw/conversations/2026-10-10-typeface-as-persona.md](../../raw/conversations/2026-10-10-typeface-as-persona.md); one verbatim user message stating the rationale

The 2026-09-14 export is a complete conversation ending on an assistant turn. The user's four acceptances above are quoted from their own messages; everything else in the conversation is the assistant's proposal. The assistant is an external session with no access to this repository's records, and one claim about JetBrains Mono Slashed is supported in the export only by an opaque search marker.
