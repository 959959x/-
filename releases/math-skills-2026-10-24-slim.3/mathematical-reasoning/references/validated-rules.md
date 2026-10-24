# 范围受限的已验证数学检查原则

source_status：R37（源 v37，2026-10-14；公开整理 2026-10-23）的 5 张范围受限 Level 3 / validated 卡，均非 strong。source_status 表示来源报告的验证状态，不代表本次独立认证。

integration_status：2026.10.24-fusion.2 将六操作字段与按需历史 Evidence 分开，保留稳定 ID、操作内容和来源 Confidence；未重做论文训练、未提升等级。MR-O001–004 延续原卡，SION-M03 从 R37 接入。历史字段中的“本次”指来源记录。

按当前任务只读取相关操作卡；需要判断来源、版本或置信依据时再读相应 Evidence。validated 不是自动定理、正确性保证或免除重算的许可。来源支持性重构和审查记录未公开，不构成可公开复现的 benchmark。相同论文多稿、来源后补算和相关作者继承不增加独立来源数。

| 当前检查责任 | 操作卡 | 按需来源证据 |
| --- | --- | --- |
| 按测试后乘积目标分配收敛责任 | [MR-O001](rules/MR-O001.md) | [Evidence](evidence/MR-O001.md) |
| 将算子、近似和测试的作用域一起核对 | [MR-O002](rules/MR-O002.md) | [Evidence](evidence/MR-O002.md) |
| 核对时间输出拓扑、覆盖范围与代表责任 | [MR-O003](rules/MR-O003.md) | [Evidence](evidence/MR-O003.md) |
| 核对否定与必要性断言的实际范围 | [MR-O004](rules/MR-O004.md) | [Evidence](evidence/MR-O004.md) |
| 有限凸生成对象的拓扑接口适配（Level 3 Validated，范围受限、非strong） | [SION-M03](rules/SION-M03.md) | [Evidence](evidence/SION-M03.md) |

SION-M03 只处理 Nikaidô/Sion 的有限凸生成拓扑接口：几何像域与系数域均可合法，不设普遍系数优先；有限凸包不自动是单纯形。源同对象重构仅覆盖两个紧凸域、实值分别连续、拟凹/拟凸范围，不扩展为 Sion 的一紧域一般性验证。

[候选库](rule-candidates.md)中只有 HEAT-FK-M01 与 EULER-CET-DR-M01 两张活动 Level 2 卡；已迁移条目只是历史指针。来源缩写见[证据来源](evidence-sources.md)，未能解开的缩写保留未核状态。
