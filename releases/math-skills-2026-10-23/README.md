# Mathematics skills: writing, reasoning and workflow

[中文说明](README.zh-CN.md) · [Version status](VERSION_STATUS.md) · [Evidence and publication limits](PUBLICATION.md) · [MIT license](LICENSE) · [License scope](LICENSE_SCOPE.md)

## Purpose

The goal is to make AI-assisted mathematical writing easier for mathematicians and other intended readers to understand **without changing the supplied mathematical content, assumptions, results or proof logic**. Readability is a goal, not a demonstrated guarantee. These skills do not certify proofs or replace qualified mathematical review.

This is a portable, instruction-only documentation bundle dated **2026-10-23**, not a trained model, software application, automated training job or paper corpus. It contains three complementary skill folders:

| Skill | Included baseline | Main responsibility |
| --- | --- | --- |
| [Mathematical Writing](mathematical-writing/README.md) | W35 | Improve exposition and organize supplied mathematics while preserving meaning and scope. |
| [Mathematical Reasoning](mathematical-reasoning/README.md) | R37 | Reconstruct or review explicitly requested mathematical arguments and distinguish checked, conditional and unresolved steps. |
| [Math Paper Workflow](math-paper-workflow/README.md) | Unnumbered snapshot; last source update 2026-10-04 | Select the appropriate task mode and coordinate mathematics, writing, source use and delivery checks. |

W36 and R38 are not included. This release does not change any rule's evidence level or confidence. Older repository releases remain separate and unchanged.

## Choose the smallest useful scope

- **Polish a paragraph or theorem:** start with [writing](mathematical-writing/SKILL.md). Keep the original language unless translation is requested; list mathematical concerns separately. A missing full proof is not a reason to refuse a narrow language edit.
- **Review or reconstruct a proof:** start with [reasoning](mathematical-reasoning/SKILL.md). Fix the mathematical object and requested claims, check relevant dependencies, and report unresolved steps. Do not silently strengthen assumptions or replace the result.
- **Organize a full manuscript or combine tasks:** start with [workflow](math-paper-workflow/SKILL.md), then load only the relevant companion and reference files.
- **Learn writing from a paper:** explicitly request a bounded learning reconstruction. The opt-in contracts require mathematical review before writing review, and both before source comparison. Ordinary editing does not trigger this process.

## Portable use

1. Keep the three skill folders together with this license and the documentation. Each folder has a `SKILL.md` entrypoint and supporting Markdown references.
2. In an assistant that supports local instruction skills, use that host's documented skill-import or folder-registration mechanism. This bundle does not install itself or claim compatibility with every client. If manually loading instructions, begin with the relevant `SKILL.md` and make its linked references available.
3. Supply the actual manuscript or mathematical statement, target reader, language, scope, permitted changes and available review baseline. Respect copyright and permission requirements for source material.
4. Ask for the requested deliverable and an honest account of what was and was not checked. Formatting, compilation and visual inspection require tools supplied by the host; unavailable checks must not be reported as passed.

No scripts, model weights, tool credentials, executable installers, external-service integrations or third-party papers are bundled. Merely copying, reading or enabling the skills does not authorize ongoing training, rule updates, publication or other external actions. If copying only one skill folder, include the license and adapt companion links without weakening its mathematical or task-scope boundaries.

## Example requests

**Same-language copy-editing:** “Polish this English theorem and its explanation for a mathematical audience. Preserve formulas, assumptions, quantifiers, conclusions and proof logic. List mathematical concerns separately; do not invent or repair a proof.”

**Proof review:** “Review this stated argument only. Identify the hypotheses used, justify the critical estimate, and distinguish checked steps from gaps. Do not add assumptions or present a repaired result as the original theorem.”

**Chinese structure editing:** “根据以下已核对的数学基线组织中文正文，说明定义、引理和主定理的位置理由。保持数学内容、假设、结论和证明逻辑，不新增研究结果，也不套固定章节模板。”

These are usage examples, not reported experimental outcomes.

## Evidence, attribution and limitations

The instruction set was developed through AI-assisted reconstruction and review. Historical “validated” and L1/L2/L3 labels retain their original scope and qualifications; they are not new independent certifications. Detailed private manuscripts and review records are excluded, so the inherited labels cannot be independently reproduced from this bundle alone. Selected public references identify source works; they do not make the private comparisons publicly reproducible.

No human-reader study, causal version advantage, guaranteed correctness, author endorsement, publication acceptance or general performance improvement is claimed. Unit-level evidence is not whole-paper validation; Chinese and English evidence are not interchangeable. Mathematical repairs must not be counted as pure prose improvements. See [PUBLICATION.md](PUBLICATION.md) and each skill's evidence notes before using its rules.

## Integrity and license

[MANIFEST.sha256](MANIFEST.sha256) lists SHA-256 checksums for every release file except the manifest itself. In an environment with `sha256sum`, run `sha256sum -c MANIFEST.sha256` from this directory to check content integrity. This checks files, not mathematics.

The original instructions and documentation in **this `releases/math-skills-2026-10-23/` subtree only** are under the [MIT License](LICENSE), copyright 2026 959959x. Linked third-party works and other repository content are not relicensed. MIT permits people to copy and modify their own copies; it does not grant direct write access to the owner's repository. This is an independent project and makes no official endorsement claim.
