---
status: confirmed
attribution: user-confirmed
updated: 2026-09-04
sources: []
---

# DEC-002 — Decision Placement

## Decision

Every decision is recorded in exactly one repository, determined by two questions asked in order.

**Question 1 — Would this decision still hold if the implementation were rebuilt in completely different technology?**

- Yes → `{project}-lab`
- No → `{project}-web`

**Question 2 — If this project ceased to exist, would this decision still apply to other TENDER SYSTEMS projects?**

- Yes → `tender-systems`

## Examples

Project Lab:

```text
narrative
brand
visual language
product concept
audience experience
project philosophy
creative decisions
```

Web implementation:

```text
framework
database
deployment
authentication
CDN
API architecture
runtime
```

Organization:

```text
repository conventions
identity policy
organization-wide principles
cross-project operating rules
```

## Rationale

A decision about the work outlives any particular implementation of it. A decision about the implementation does not. Keeping them in one repository would mean that rebuilding the implementation either destroys the reasoning behind the work or preserves obsolete technical choices alongside it.

## Consequences

- Implementation repositories carry technical documentation only. Project philosophy placed there is misfiled.
- The organization repository carries no project-specific material.
- When a decision is ambiguous, Question 1 is decided first; it is the more common case.
