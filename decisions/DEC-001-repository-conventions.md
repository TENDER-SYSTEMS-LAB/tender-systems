---
status: confirmed
attribution: user-confirmed
updated: 2026-09-04
sources: []
---

# DEC-001 — Repository Conventions

## Decision

Repositories are named in lowercase kebab-case and take one of three forms:

```text
tender-systems          organization-level conventions and project index
{project-slug}-lab      a project's knowledge, research, decisions, and memory
{project-slug}-web      a project's web implementation
```

A project's Lab repository is created when the project begins. Its implementation repository is created only when implementation actually begins.

## Rationale

A repository marks the boundary of something that exists and changes independently, not a folder for sorting files. A project's thinking and a project's implementation change on different schedules, for different reasons, and survive each other; they are separate repositories.

Empty implementation repositories are not created in advance. An architecture diagram is not a reason to create a repository.

## Consequences

- `other-goods-web` and `longing-web` do not exist and should not be created until their implementations start.
- Shared abstraction repositories — a design system, a shared UI library, a platform layer — are not created preemptively. Extract one only after the same need appears in two or three projects.
- Existing repositories are not renamed to satisfy this convention retroactively. The convention governs new repositories.
