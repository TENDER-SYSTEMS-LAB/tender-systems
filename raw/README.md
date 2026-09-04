# Raw Layer

`raw/` is this repository's Source of Truth. Preserve its materials as immutably as possible. Once a file has been added, do not edit it. If content must be corrected or extended, add a separate revision file instead of changing the existing one.

`raw/` is not the Wiki. No matter how well material has been organized or interpreted in `wiki/`, never use it to replace an original in `raw/` or to justify deleting raw material. The Wiki is an interpretive layer built on raw sources; it cannot substitute for them.

## Language

Raw sources retain the language in which they were originally created. The repository's English-default policy applies to this guide, the source registry, and all Wiki synthesis, but never authorizes translating or rewriting a registered source in place. When English access is needed, write an English synthesis in the Wiki or add a separately registered translation without modifying the original.

## Subdirectories

- **`conversations/`** — Exports of conversations with LLMs.
- **`documents/`** — Plans, briefs, instructions, and other documents written directly by the user.
- **`surveys/`** — Responses in which several LLMs independently respond to the same question. Preserve each response as `llm-proposed`; agreement among them is not a user decision.
- **`inbox/`** — Temporary storage for material that has not yet been classified or reviewed. Treat anything in `inbox/` as not promoted to the Wiki.

## File Naming

Use `YYYY-MM-DD-kebab-case-slug.md`. When adding multiple files on the same date, distinguish them with `-2`, `-3`, and so on.

## Source Registration

Every new source added under `raw/` must also be registered in `raw/sources.md`. An unregistered source is treated as nonexistent.

## Scope

This repository's raw layer holds only institution-level material: sources about TENDER SYSTEMS itself, its conventions, its public identity, and research shared across several systems. Material specific to a single system belongs in that system's Lab repository, which is its canonical source for that material. Do not copy a Lab repository's raw source here.

## Current-State Notes

As of 2026-09-05, the raw layer was created empty during the repository's alignment to the shared Wiki architecture. No source has been registered.
