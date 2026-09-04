---
status: working
attribution: user-confirmed
updated: 2026-09-05
sources: []
---

# Institutional Overview

## Definition

TENDER SYSTEMS is the institution under which individual systems are developed and operated. Its public-facing description on record is "Systems for things that resist measurement." Its GitHub organization is `TENDER-SYSTEMS-LAB`. It currently operates two active systems, OG-001 OTHER GOODS and LN-001 LONGING; see [[registry]].

## Operating Principles

Derived from the recorded institutional decisions:

- A repository marks the boundary of something that exists and changes independently, not a folder for sorting files ([[DEC-001-repository-conventions]]).
- A system's thinking and its implementation are separate repositories, created on different schedules ([[DEC-001-repository-conventions]]).
- Every decision is recorded in exactly one repository, determined by whether it would survive a full rebuild of the implementation and whether it would still apply if the system ceased to exist ([[DEC-002-decision-placement]]).
- Shared abstractions are extracted only after the same need appears in two or three systems, not created preemptively ([[DEC-001-repository-conventions]]).
- Public source control carries the identity of the practice, not of whoever was at the keyboard ([[DEC-003-public-identity]]).

## Knowledge Architecture

Every TENDER SYSTEMS repository uses the same three-layer LLM Wiki: `raw/` as source of truth, `wiki/` as synthesis, and `schema.md`/`AGENTS.md` as the operating layer. This repository is the institutional layer; each Lab repository is canonical for its own system.

## Public Identity

Public-facing authorship is `TENDER SYSTEMS`, and documents are written as institutional records rather than personal ones; see [[DEC-003-public-identity]].

## Related

- [[registry]]
- [[current-state]]
- [[DEC-001-repository-conventions]]
- [[DEC-002-decision-placement]]
- [[DEC-003-public-identity]]

## Sources

No raw source is registered yet. This page synthesizes the three recorded institutional decisions and the public-facing description of TENDER SYSTEMS.
