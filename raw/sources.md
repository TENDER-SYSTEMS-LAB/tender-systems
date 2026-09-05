# Raw Source Index

This document is the registry for every raw source. It tracks each source's ID, path, hash, and ingestion status. Any Wiki content followed back through its provenance must ultimately lead to an original through this table.

## Registration

When adding a source, append one row to the table below and record the result of `git hash-object <path>` in the `Hash` column. If a later hash differs from the registered value, the original has changed. Do not update the Wiki automatically. Mark the pages that rely on the source `REVIEW_REQUIRED` so that a person can review them again.

## Source List

| Source ID | Path | Type | Date | Attribution | Hash | Ingested | Wiki Status |
|---|---|---|---|---|---|---|---|
| `SRC-2026-09-04-apple-design-skill-review` | [raw/conversations/2026-09-04-apple-design-skill-review.md](conversations/2026-09-04-apple-design-skill-review.md) | conversation | 2026-09-04 | llm-proposed | `6bf98420ba45c7f49ee13fbe25d001c714878a8c` | 2026-09-05 | partially promoted |
| `SRC-2026-09-04-tender-systems-identity-review` | [raw/conversations/2026-09-04-tender-systems-identity-review.md](conversations/2026-09-04-tender-systems-identity-review.md) | conversation | 2026-09-04 | jointly-developed | `d6e5cf6895846d41e684d9a55b2ec5b9d9a90df9` | 2026-09-05 | partially promoted |
| `SRC-2026-09-05-social-account-strategy` | [raw/conversations/2026-09-05-social-account-strategy.md](conversations/2026-09-05-social-account-strategy.md) | conversation | 2026-09-05 | jointly-developed | `8a5a64971d40d8cb49a8ac2e5d911fb52d192424` | 2026-09-05 | partially promoted |
| `SRC-2026-09-05-how-to-show` | [raw/conversations/2026-09-05-how-to-show.md](conversations/2026-09-05-how-to-show.md) | conversation | 2026-09-05 | llm-proposed | `a9fc7d974ce281c885da0c855e1348ca74374dd5` | 2026-09-05 | partially promoted |

## Provenance notes

`SRC-2026-09-04-apple-design-skill-review` — The external repository it reviews (`dickwu/apple-design-skill`) is not registered here and is known only through the assistant's summary. The conversation ends with no user response, so nothing in it is user-confirmed.

`SRC-2026-09-04-tender-systems-identity-review` — The assistant's opening synthesis draws on earlier conversations that are not registered in this repository, and the operational rules in the final exchange arrive inside an instruction block the user pasted from work done elsewhere; both are secondary citations. The file contains the operator's personal name and is retained unchanged as evidence; that name is not carried into the Wiki.

`SRC-2026-09-05-social-account-strategy` — The assistant used live web search and cited external help-centre and newsroom pages that are not registered here; platform facts in it were true as reported on 2026-09-05 and need re-verification. The final live account handles are not stated by the user in the transcript.

`SRC-2026-09-05-how-to-show` — The supplied excerpt contains recommendations in an assistant voice, without role labels, the initiating user prompt, or a user reply. No proposal is user-confirmed. External platform links are secondary references and were not verified during ingestion; platform claims and submission recommendations remain in raw.
