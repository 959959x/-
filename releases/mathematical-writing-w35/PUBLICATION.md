# Public packaging notes

Release: W35 public edition. Packaging date: 2026-10-21. This is a distribution edit, not a mathematical or writing-rule update.

## Preserved

- Stable rule IDs; the six operational fields and Confidence text for MW-O001, MW-O002, MW-O003 and the KM86-W03 candidate.
- L1/L2/L3 distinctions, the MW-O004 merge status, non-strong qualifications, language limits and warnings against causal overclaims.
- Mathematical-preservation checks, the ordering of mathematical and writing audits, source-exposure honesty, and task routing that keeps ordinary copy-editing lightweight.
- The manuscript-editing reference unchanged.

## Changed for public distribution

- Replaced detailed case-by-case Evidence narratives with explicitly limited public summaries and selected bibliographic links. The summaries are not a reproducibility dataset or independent certification.
- Replaced the historical legacy inventory with a general classification note, without individual manuscript or relationship details.
- Generalized the named-group style route into user-specified reference-style guidance.
- Made the separate reasoning skill optional while retaining mathematical-review responsibility.
- Rephrased personalized ongoing-work and log instructions as explicit task-scoped behavior.
- Simplified optional UI metadata and omitted the earlier icon because its redistribution rights were not established.
- Added English and Chinese usage guides, provenance/evidence limits, selected bibliography, manifest and the owner-approved MIT license scoped to this new release directory.

## Not included

Private drafts, raw conversations, detailed audit reports, coordination records, absolute workspace paths, credentials, personal contact information, third-party paper PDFs or figures, unpublished W36 changes, a bundled reasoning skill, and application claims or metrics.

No new evaluation is claimed. Structural validation and a preservation comparison can check package shape and unchanged fields, but do not establish mathematical correctness or better writing outcomes.

## File map

- `README.md`: English overview, installation, examples and limits.
- `README.zh-CN.md`: concise Chinese usage guide.
- `LICENSE`: MIT, scoped as described in the README.
- `MANIFEST.sha256`: hashes of every release file except this manifest itself.
- `mathematical-writing/SKILL.md`: skill entrypoint.
- `mathematical-writing/agents/openai.yaml`: optional UI metadata.
- `mathematical-writing/references/language-routes.md`: separate language routes.
- `mathematical-writing/references/manuscript-editing.md`: full-manuscript checklist.
- `mathematical-writing/references/training-contract.md`: opt-in paper-learning protocol.
- `mathematical-writing/references/validated-rules.md`: three scoped rule cards.
- `mathematical-writing/references/rule-candidates.md`: candidate and ID migration record.
- `mathematical-writing/references/legacy-evidence-inventory.md`: classification boundaries.
- `mathematical-writing/references/evidence-notes.md`: public evidence and provenance limits.
- `mathematical-writing/references/bibliography.md`: selected primary-source references.
- `PUBLICATION.md`: this change summary.
