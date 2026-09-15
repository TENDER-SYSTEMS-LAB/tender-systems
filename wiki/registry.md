---
status: confirmed
attribution: user-confirmed
updated: 2026-09-15
sources:
  - SRC-2026-09-15-longing-research-rename
  - SRC-2026-09-15-reserve-absorption-and-trust-instruments
  - SRC-2026-09-07-the-reserve-identifier-confirmation
---

# System Registry

This page is the canonical catalog of the systems TENDER SYSTEMS operates. It records each system's identifier, name, status, repositories, and one-line description. It does not summarize a system's content — each system's Lab repository is the canonical source for that.

| System ID | Name | Status | Lab Repository | Implementation | Description |
| --- | --- | --- | --- | --- | --- |
| OG-001 | OTHER GOODS | active | [other-goods-lab](https://github.com/TENDER-SYSTEMS-LAB/other-goods-lab) | not created | An interactive conceptual art system in which a commerce interface treats things that cannot be owned or delivered as merchandise. |
| LN-001 | LONGING RESEARCH | active | [longing-lab](https://github.com/TENDER-SYSTEMS-LAB/longing-lab) | not created | An interactive system presented as a fictional research house that prices conditions of human experience that modernization is removing. |
| RS-001 | THE RESERVE | archived | [the-reserve-lab](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab) | none | A place for what remains. Concluded 2026-09-15; its function passed to LN-001. |

## OG-001 — OTHER GOODS

- System ID: OG-001
- Name: OTHER GOODS
- Status: active
- Lab repository: [other-goods-lab](https://github.com/TENDER-SYSTEMS-LAB/other-goods-lab)
- Implementation repository: not created yet
- Description: an interactive conceptual art system in which a commerce interface treats things that cannot be owned or delivered as merchandise.

The Lab repository is the canonical source for everything about this system. This page does not restate its content.

Related institutional documents:

- [[DEC-001-repository-conventions]]
- [[DEC-002-decision-placement]]
- [[DEC-003-public-identity]]
- [[overview]]

## LN-001 — LONGING RESEARCH

- System ID: LN-001
- Name: LONGING RESEARCH
- Former name: LONGING, until 2026-09-15
- Status: active
- Lab repository: [longing-lab](https://github.com/TENDER-SYSTEMS-LAB/longing-lab)
- Implementation repository: not created yet
- Description: an interactive system presented as a fictional research house that prices conditions of human experience that modernization is removing.

The Lab repository is the canonical source for everything about this system. This page does not restate its content.

On 2026-09-15 the user renamed the system from **LONGING** to **LONGING RESEARCH**, on the stated rule that each work in the series carries a two-word name. The naming rationale and the precedent it reverses are canonical in [the Lab's naming decision](https://github.com/TENDER-SYSTEMS-LAB/longing-lab/blob/main/wiki/decisions/DEC-001-project-name-longing.md).

The identifier `LN-001` is unchanged: identifiers are assigned once and are neither reused nor re-derived when a name changes. The Lab repository is still `longing-lab` and the public accounts are still registered under `LONGING`; neither was renamed, and both are open questions. See [[public-surfaces]].

Related institutional documents:

- [[DEC-001-repository-conventions]]
- [[DEC-002-decision-placement]]
- [[DEC-003-public-identity]]
- [[overview]]

## RS-001 — THE RESERVE

- System ID: RS-001
- Name: THE RESERVE
- Status: archived — concluded 2026-09-15
- Lab repository: [the-reserve-lab](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab)
- Implementation repository: none; never created
- Public description: A place for what remains.

On 2026-09-07, the user requested inclusion under ACTIVE SYSTEMS and explicitly confirmed RS-001 — THE RESERVE, with README and Wiki updates in both repositories. The project name and identifier decision is canonical in [THE RESERVE's naming decision](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab/blob/main/wiki/decisions/DEC-001-project-name.md); its public bio is documented in [the public-language decision](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab/blob/main/wiki/decisions/DEC-002-public-language.md). Project mechanisms and social handles remained outside that registration.

On 2026-09-15 the user directed that the system be shown as ended. RS-001 is the first `archived` system. Its function — what a value is stored in, and what backs the things that rest on it — passed to LN-001, where it is carried by two instruments named BEARER BOND and BLIND TRUST. The monetary design developed under RS-001 did not transfer and is preserved unedited in its Lab.

The conclusion is canonical in [THE RESERVE's conclusion decision](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab/blob/main/wiki/decisions/DEC-012-system-concluded-and-function-transferred.md) and its inheritance in [LONGING's absorption decision](https://github.com/TENDER-SYSTEMS-LAB/longing-lab/blob/main/wiki/decisions/DEC-006-reserve-function-absorbed.md). This registry records the status change only; the reasoning stays in the Labs, per [[DEC-002-decision-placement]]. The identifier RS-001 is not released and is never reused.

## Status Values

- `active` — Currently operated and developed.
- `paused` — Temporarily not being developed, expected to resume.
- `archived` — Concluded and no longer developed.
- `proposed` — Identified but not yet begun.

RS-001 became the first `archived` system on 2026-09-15. Archiving marks a system concluded; it does not delete its Lab, release its identifier, or resolve the questions it left open.

## Identifier Scheme

A system identifier is a two-letter system prefix derived from the system name, followed by a zero-padded three-digit sequence number. An identifier is assigned once and never reused. A rename does not re-derive it: `LN-001` was derived from LONGING and is retained under LONGING RESEARCH. The three current identifiers, `OG-001`, `LN-001`, and `RS-001`, are on record; no rule beyond this is decided.

## Adding a System

Create `{project-slug}-lab` first. Create `{project-slug}-web` only when implementation actually begins. Register the system here in the same task. See [[DEC-001-repository-conventions]].

## Boundary

This registry stores registry-level facts and cross-system relationships only. A system's research, narrative, concepts, and creative decisions stay canonical in its Lab repository. See [[DEC-002-decision-placement]].

## Sources

- [[SRC-2026-09-07-the-reserve-identifier-confirmation]] — [raw/conversations/2026-09-07-the-reserve-identifier-confirmation.md](../raw/conversations/2026-09-07-the-reserve-identifier-confirmation.md)
