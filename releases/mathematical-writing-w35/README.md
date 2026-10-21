# Mathematical Writing · W35 public edition

A writing skill for mathematical papers, especially PDE and analysis: organize checked mathematics, improve Chinese or English exposition, and keep mathematical correctness separate from prose quality.

This is a **writing-only, instruction-only release** based on the stable W35 snapshot. It contains no model weights, executable scripts, external-service integration or paper corpus. W36 is not included.

[中文指南](README.zh-CN.md) · [Skill entrypoint](mathematical-writing/SKILL.md) · [Evidence limits](mathematical-writing/references/evidence-notes.md) · [License](LICENSE)

## What it does

- Copy-edit in the original language without silently changing mathematical claims.
- Translate only when asked, preserving hypotheses, quantifiers and uncertainty.
- Organize a manuscript by actual proof dependencies and reader needs, not a fixed chapter template.
- For explicitly requested paper-learning exercises, separate mathematical reconstruction, independent writing, mathematical audit, writing audit and source comparison.

A paragraph edit does **not** automatically start a proof audit, translation or paper-training exercise. This is not a theorem prover, correctness certificate or substitute for qualified mathematical review.

## Install in Codex

Copy the entire `mathematical-writing/` folder into your project's `.agents/skills/` directory, so the entrypoint is `.agents/skills/mathematical-writing/SKILL.md`. For a user-wide installation, use `$HOME/.agents/skills/mathematical-writing/` instead. Keep an existing installation backed up and avoid installing duplicate skills with the same name.

In Codex CLI or the IDE extension, select it through `/skills` or mention `$mathematical-writing`. Codex normally detects changes automatically; restart if it does not appear. These are local folder instructions, not a marketplace/plugin installation. See the [official skill documentation](https://learn.chatgpt.com/docs/build-skills) for current client-specific behavior.

## Examples

**Copy-edit without scope expansion**

> Use $mathematical-writing to polish the following English theorem and paragraph. Keep the language English and preserve all assumptions, quantifiers, endpoints and claims. List mathematical concerns separately; do not invent a proof.

**中文结构编辑**

> 使用 $mathematical-writing，根据下面已经核对的定理和证明骨架组织中文正文。先给出主要定义、引理与定理的位置及理由，再写正文。不要新增研究结论，也不要套固定章节模板。

**Explicit learning reconstruction**

> Use $mathematical-writing for a learning reconstruction of this specified proof unit. Fix the mathematical scope and source version first. Preserve the source-closed writing and audit sequence, disclose prior source exposure, and compare with the source only after both audits. Do not update rules without a separate explicit request.

## Mathematical-review dependency

A separately installed `mathematical-reasoning` skill is optional and is not bundled. Ordinary copy-editing and translation do not require it. If the requested task genuinely includes proof reconstruction or correctness review, use a suitable available mathematical reviewer or carry out the checks specified in [the training contract](mathematical-writing/references/training-contract.md). If the mathematics cannot be checked, report that boundary instead of labelling the audit passed. The absence of a companion skill does not waive the audit gate.

LaTeX compilation and visual PDF checking require tools supplied by the execution environment; this package does not install them. An unavailable check must be reported, not silently marked complete.

## Provenance and limits

The workflow was developed with AI-assisted mathematical reconstruction and review. The three scoped L3/validated rules and one L2 candidate retain their W35 classifications and qualifications; packaging adds no training result, rule upgrade or performance claim. Detailed training drafts and audit records are not included, so those inherited classifications are **not independently reproducible from this public package**. Selected primary references remain linked for attribution.

No human-reader study, benchmark success rate, publication acceptance, author endorsement or general superiority of a newer version is claimed. Inspect the [evidence notes](mathematical-writing/references/evidence-notes.md) before treating a rule as applicable. The README examples illustrate intended usage; they are not reported experiment results.

## Release contents and scope

See [PUBLICATION.md](PUBLICATION.md) for the packaging changes and [MANIFEST.sha256](MANIFEST.sha256) for file hashes. This directory is an additive release: it does not replace or relicense the repository's earlier original or fusion versions.

## License and repository access

The newly added, original skill instructions and documentation **within this `releases/mathematical-writing-w35/` subtree** are licensed under the [MIT License](LICENSE), copyright 2026 959959x. This license does not relicense older repository content, linked third-party publications or other third-party material. No third-party paper text or figures are distributed here.

MIT permits reuse and modification of copies; it does not grant direct write access to this repository. Repository write permissions remain under the owner's control. This is an independent project, not an OpenAI-endorsed skill or a claim of acceptance into any support program.
