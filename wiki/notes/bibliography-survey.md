---
status: working
attribution: llm-synthesis
updated: 2026-09-08
sources:
  - SRC-2026-09-08-bibliography-survey
  - SRC-2026-09-08-human-social-engineering-models
---

# Bibliography Survey

On 2026-09-08, the user asked an assistant to search for artworks and papers usable as references for the work, instructing it to read the wikis under the organization's repositories first to confirm the shared worldview and each work's concept. The English below renders the Korean original:

> "Search the internet for artworks and papers that could be used as references for my work. Read the wikis under https://github.com/TENDER-SYSTEMS-LAB and check the worldview or the work's concept, and find them on that basis."

In a second turn the same day, the user widened the scope beyond art to social-science, humanities, and engineering papers that model human or social phenomena mathematically:

> "@GitHub Even if they are not necessarily art-related papers, are there social-science or humanities papers that tried to work out a social phenomenon or something human through a mathematical model? Or go ahead and find papers in the engineering field as well."

The conversation ends on the assistant's second answer. No user reply to either turn appears in the export, and nothing the assistant proposed is adopted, selected, or confirmed anywhere in the source.

## Institution-level references proposed

Attribution: `llm-proposed`. Item, creator or author, year, and the one-line reason given in the source:

- Wendy Nelson Espeland and Mitchell L. Stevens, "Commensuration as a Social Process" (1998) — offered as the strongest cross-cutting theoretical starting point for all systems.
- Carrie Lambert-Beatty, "Make-Believe: Parafiction and Plausibility" (2009) — how a fiction is accepted as real inside a real context.
- Marcel Broodthaers, "Musée d'Art Moderne, Département des Aigles" (1968–1972) — institution as the medium rather than the backdrop.
- Dylan Hadfield-Menell and others, "Inverse Reward Design" (2017) — proposed as fitting the institution as a whole.
- David Gale and Lloyd Shapley, "College Admissions and the Stability of Marriage" (1962) — what a working system actually guarantees.
- Paolo Cirio, "Loophole for All" (2013), and Goldin+Senneby, "Headless" (from 2007) — each tied to one system and to the institution together, so cross-system rather than institution-only.
- A design-research methodology cluster: John Zimmerman, Jodi Forlizzi, and Shelley Evenson, "Research through Design as a Method for Interaction Design Research in HCI" (2007); William Gaver, "What Should We Expect from Research through Design?" (2012); Phoebe Sengers and others, "Reflective Design" (2005) — offered as a route from a decision record to research.

## Per-system references

The survey produced roughly twelve artworks and thirty-three papers in total. Beyond the institution-level items above, most of the remainder is scoped to a single system rather than to the institution as a whole — the larger part assigned to LN-001, with smaller sets assigned to OG-001 and RS-001. This page does not list those per-system items. Each system's Lab repository remains canonical for its own prior art and bibliography:

- [other-goods-lab](https://github.com/TENDER-SYSTEMS-LAB/other-goods-lab)
- [longing-lab](https://github.com/TENDER-SYSTEMS-LAB/longing-lab)
- [the-reserve-lab](https://github.com/TENDER-SYSTEMS-LAB/the-reserve-lab)

## Annotated bibliography document

The Markdown annotation file generated during that session was supplied afterwards and is registered as `SRC-2026-09-08-human-social-engineering-models`. It annotates the twenty social-science and engineering papers from the second turn with a field, a description of what each model covers, a proposed connection to the work, stated assumptions and limits, the assistant's own verification scope, a DOI, and a BibTeX key. Its content is largely derived from the conversation rather than new, and it states its own status as a research reference proposal that is not a design decision, an implementation, or an empirical validation. It also lists the specific repository files it claims to have read, which narrows the conversation's otherwise unsupported claim of repository access without closing it.

Two of its passages are institution-level rather than scoped to one system, and both are `llm-proposed`:

- **A reading discipline.** It separates three kinds of model and states what each does and does not establish: a theoretical explanatory model analyses what follows from stated assumptions and is not a universal law; a data- or experiment-based model is judged by how well it explains or predicts a particular observation, and transfer to another subject or time unit requires separate validation; an algorithmic or engineering theorem states what a rule guarantees, and that guarantee is not the whole of human desirability.
- **A research record discipline.** It proposes that, when a model is applied, the record keep the original state variables, units, and assumptions separate from what the work changes, from the rules by which synthetic data is generated, and from real observation. It further distinguishes quantities that are easily conflated — how often a practice occurs, how much attention it receives, what an individual values it at, what an institution estimates, and what a market prices it at — and notes that reproducing a curve does not establish what produced it.

Neither discipline has been adopted. They are recorded here because they would apply across systems if adopted, unlike the per-system reading proposals in the same document. The document's proposed separation structure for one system's information and pricing layers is scoped to that system and stays canonical in its Lab repository.

## Status

Everything recorded above is `llm-proposed`. The user neither selected, endorsed, nor rejected a single artwork, paper, or interpretive link in either turn. This page records that a survey was produced and what its institution-level portion contains; it does not establish a reading list, a citation plan, or a research direction.

## Verification limits

The assistant ran web searches with visible result sets and supplied a link or DOI for nearly every item, but the descriptions attached to each item are its own summaries and were not independently checked during ingestion. It self-reported checking only the bibliography, not the full text, for Hartmut Rosa (2003), and self-reported checking only the publisher listing and table of contents, not the body, for Christopher Williams-Wynn (2025) because of access restriction. A Kalman filter formulation it reproduced is explicitly marked in the source as a modernised, simplified notation rather than a transcription of the original. Two of the supplementary papers cited in the second turn's body — including Fehr and Schmidt (1999) — are missing from that turn's own closing source list. The assistant asserts in prose that it read the organization's repository wikis, including a claim about a 120-item list held in one Lab repository's wiki, but no repository URL, page title, or quoted wiki text appears anywhere in the export, so both the general claim and that specific list are unverifiable from this file. Of the two files it generated, the Markdown annotation file was later supplied and is registered as `SRC-2026-09-08-human-social-engineering-models`; the BibTeX file is not registered. In that annotation file the per-item verification scope is the assistant's own account and was not rechecked during ingestion, several reproduced formulations are marked in the source itself as simplified or modernised notation, and one worked arithmetic example is described there as an illustration for the work rather than an estimate taken from the cited paper.

## Related

- [[tender-subject-systematic-form]]
- [[academic-guidance-and-publication]]
- [[Q-002-internal-versus-public-language]]
- [[current-state]]

## Sources

- [[SRC-2026-09-08-bibliography-survey]] — [raw/conversations/2026-09-08-bibliography-survey.md](../../raw/conversations/2026-09-08-bibliography-survey.md)
- [[SRC-2026-09-08-human-social-engineering-models]] — [raw/documents/2026-09-08-human-social-engineering-models.md](../../raw/documents/2026-09-08-human-social-engineering-models.md)

The design-research references in this survey concern audience interpretation and research methodology, not a shared visual or interaction design system, and must not be read as material for [[Q-001-shared-design-system]].
