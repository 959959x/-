# 数学论文写作：W35 公开版

这份技能用于中文或英文数学论文的润色、明确要求的翻译、结构编辑，以及明确要求的证明驱动学习。核心是：写清楚已有数学，不暗改假设、量词、参数端点或结论；数学正确性与文字质量分别检查。

## 安装和调用

将完整的 `mathematical-writing/` 文件夹复制到项目的 `.agents/skills/`，使入口为 `.agents/skills/mathematical-writing/SKILL.md`。个人通用安装可放到 `$HOME/.agents/skills/mathematical-writing/`。备份已有版本，避免同时安装同名技能。

在 Codex CLI 或 IDE 扩展中使用 `/skills` 选择，或在提示词中写 `$mathematical-writing`。当前安装方式见[官方文档](https://learn.chatgpt.com/docs/build-skills)。这是一份可本地安装的技能目录，不是已上架插件。

## 可直接使用的请求

- “使用 $mathematical-writing 润色下面的中文段落，保留数学内容，不翻译；数学疑点另列。”
- “使用 $mathematical-writing 将下面的英文定理翻译成中文，保留全部量词、条件、公式和未证状态。”
- “使用 $mathematical-writing 根据这份已核证明骨架组织英文正文，说明定义与引理的摆放理由，不新增结果。”

仅当明确要求论文学习训练时，才启用完整的数学重构、来源关闭、独立写作、数学审查、写作审查和来源比较流程。普通润色不自动升级为整篇核验。

## 内容与边界

- 基线为稳定W35，不包含W36，也没有因公开打包而新增或升级规则。
- 三条核心规则仍是范围受限L3/validated，非strong；KM86-W03仍是L2候选。操作字段与Confidence原文保留。
- 原始训练稿件和逐轮审查记录未公开，因此不能仅凭本包独立复现历史证据等级；文献链接只用于准确归属，不构成数学认证。
- 不声称人类读者实验、成功率、新版整体胜出、原作者背书或新数学发现。
- `mathematical-reasoning` 是可选配套，不在包内。确需数学审查时必须完成相应检查；缺少配套技能或工具不能被写成已经通过。
- LaTeX编译和PDF逐页检查依赖运行环境；未完成的检查须如实披露。

详见[英文说明](README.md)、[公开证据边界](mathematical-writing/references/evidence-notes.md)与[发布改动清单](PUBLICATION.md)。

## 许可与权限

MIT许可证仅适用于本次新增的 `releases/mathematical-writing-w35/` 子目录内的原创技能说明与文档，不重新授权仓库旧原版、融合版或第三方论文。版权署名为2026 959959x。

MIT允许他人复制、修改其自己的副本及商业使用，但不赋予他人直接修改本仓库的权限。本项目不代表OpenAI官方背书或活动申请获批。
