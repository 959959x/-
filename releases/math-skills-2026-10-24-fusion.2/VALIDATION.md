# 集成验证记录

状态：集成与限定行为验证通过（2026-10-24）。

已将固定提交的35个上游输入文件按 Git blob SHA 核对，并逐项通过上游 MANIFEST.sha256。已保存三个本地技能的35个文件基线及 SHA-256；候选包从该副本建立。

静态检查149项通过：三个技能的 quick_validate、原有文件保留、UI/图标/自动调用、Nature 两模块与旧来源附录、上游许可原文、5张推理卡及3条写作规则的操作字段、来源 Evidence/Confidence、L2候选边界、训练契约一致性、相对链接和公开路径检查。Euler 的 Use when 按计划保留本地任务适用条件，其余对应字段按上游核对。

三个版本各执行同一组9项任务，27份实际交付经核查，在指定语言、数学条件与任务范围内均通过；未发现融合版在这些场景中的回退。独立静态审阅未发现安装或发布阻塞。见[行为核查与限制](validation/assessment.md)、[任务材料](validation/cases.md)、[独立审阅](validation/independent-review.md)和[静态检查](validation/static-checks.json)。

- [旧融合版实际答案](validation/results-baseline.md)
- [公开版实际答案](validation/results-upstream.md)
- [本次融合版实际答案](validation/results-fusion.md)

这不是新版优越性的统计证明；部分题目未实际载入相关可选写作卡，不能反推该卡产生了收益。此次没有新的论文训练或证据等级升级。安装后文件哈希与远端旧版本保留情况另在交付时核对。
