# 当前融合：2026.10.24-fusion.2

本次以 2026.10.10-fusion.1 的本地三技能为基线，接入[固定 W35/R37 公开包](https://github.com/959959x/-/tree/eb6f8130f67d2fb8c4d4d552985144d4412edde1/releases/math-skills-2026-10-23)。写作 MW-O002 的操作增量、推理 SION-M03 及更新后的公开 Evidence 各保留来源适用范围；继承的等级不代表本次重训。当前集成验证另见发行包 VALIDATION.md。

research-framing.md 与 journal-adaptation.md 沿用上一版内容；以下快照记录原始来源与历史验证边界。当前规则内容以本版规则卡为准，下面“保持原始内容”等描述仅指 2026-10-10 的那次融合。

---

## 历史记录（2026-10-10 原文）

# 融合来源与边界

## 版本与实际修改

- 日期：2026-10-10（Asia/Shanghai）。本发行号：2026.10.10-fusion.1。
- 数学包基线：959959x/-，commit `40ea90ddf14eda1202fde85745d51cef2993b0c6`。来源：[固定版本](https://github.com/959959x/-/tree/40ea90ddf14eda1202fde85745d51cef2993b0c6)。全部37个输入文件已按Git blob SHA核对。
- Nature写作参考：本机nature-writing，manifest标记1.5.0；使用的文件快照SHA-256见下表。引用文件用于此次改写，安装运行不依赖本机Nature目录。
- 新增`research-framing.md`和`journal-adaptation.md`；mathematical-writing入口按任务加载，math-paper-workflow添加转入指引。普通成稿读取授权材料与训练闭源阶段分开。
- mathematical-reasoning、所有原有validated-rules、rule-candidates和training-contract保持原始内容；原有规则ID、证据等级和适用条件没有升级或删除。
- README与包完整性清单同步更新；技能显示元数据和自动调用策略保持原样。

## 采用与改写的内容

| 来源内容 | 融合后的处理 | 身份 |
|---|---|---|
| 摘要与正文一致、精确贡献、文献关系 | 以数学基线和具体适用条件落实 | 编辑建议 |
| 引言问题与缺口 | 改为已有定理范围、当前障碍与本文已建立的结果 | 待验证迁移建议 |
| 精简摘要的证据链 | 保留定义结果的条件与关联主结果；证明创新仅在已给时使用 | 待验证迁移建议 |
| 意义、边界与解释强度 | 区分定理、严格推论、数值观察、猜想和缺口 | 编辑与任务保持约定 |
| 正文压缩和SI分配 | 遵守已有数学全文编辑规则；保留证明责任与准确调用 | 编辑建议，非默认SI规则 |
| 期刊风格与投稿 | 仅在要求时适配；精确要求核当前官方指南 | 可选工作模块 |

不默认迁移实验发现顺序、消融、统计模板、固定章节/段数、单中心主张上限、过去时要求、中文转英文默认或整包always_load。不会因为移植Nature经验而将其标为L2/L3；一般操作约定、用户偏好、期刊硬规定和文献归纳的写作规律分别记录。

## 验证和训练边界

本次的结构校验与独立行为试验，只评价安装包及选定任务的表现；不构成整篇PDE证明认证、跨论文训练或L3升级。行为输出及实际检查报告单独交付，不把预期结果写成已通过。

后续升级仍需按原训练契约记录来源、适用/不适用条件、独立性和真实结果；来源开放阶段及旧/新盲测顺序不变。通用融合模块不能授权提前读本轮测试论文。新增规则如果失败，应修订或撤回；不能通过后补历史来宣称此前已验证。

## 参考快照

文件名和散列是此次融合来源记录，不是需在目标机安装的依赖。Nature语料归纳不是官方期刊政策；此处没有重新认证引用论文的证明或声称此次完整阅读了它们。

| 参考文件 | SHA-256 |
|---|---|
| `nature-writing/manifest.yaml` | `2a0fa0108f6f740183711221311c4323a8bcd783a8291fa41efa28e6ff365014` |
| `nature-writing/static/core/stance.md` | `ebe691909f4aef282e0d976565fb08ec2b41e62b72f464629c9781d732c53326` |
| `nature-writing/static/core/workflow.md` | `e02426a89e729d6f725d83a4ad41f8393a3aa0fcd968c7a0402a0e2b6b6293fd` |
| `nature-shared/core/nature-abstract.md` | `92c0f1e78df5a9b4dc7ad276ed625e371d211124a47a9eed0a4de82c9c1526cb` |
| `nature-shared/core/nature-introduction.md` | `813fb8acb9b5c76e9c8f1d8c1616fefa82a1ec949d4aba98935b0485fb4cd4f7` |
| `nature-shared/core/nature-results-discussion.md` | `16f1ce1ed6d2aad7853eabf304cdbd661530931747bce4cf3f10b3dfb655adc1` |
| `nature-shared/core/discussion-argument-language.md` | `a3b0ddcadc47efc029e923ae8133ba0bd99e6a6eb27fdbc791d0e1096d98c169` |
| `nature-shared/core/main-text-discipline.md` | `d43190c4d617096c1088bb5452cec5b0ae13f5d4947c2b21c28315181f051b8e` |
