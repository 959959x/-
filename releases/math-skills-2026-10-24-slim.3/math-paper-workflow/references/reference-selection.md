# 范围限定的数学写作参考选择

本指南用于选择与当前稿件相符的参考材料，不记录私人来源、阅读历史、作者关系或个人偏好。下列做法是可检验的编辑建议，不是对某一群体或全部数学论文的观察结论。

## 1. 固定用途，再选择材料

- 分开数学基线、风格参考、排版模板和待评价修订稿。风格参考不得覆盖数学基线。
- 按问题类型、证明机制、读者和目标语言选择可读取且有权使用的来源。作者声望、合作关系或刊物名不能替代内容核查。
- 为每个来源写明使用范围：引言定位、定理布局、关键估计叙述、长证明组织或理论与数值的区分。不要将一篇的全部结构设为通用模板。
- 正式引用前核对作者、题名、年份、版本、DOI 与定位。区分 PDF 页码和印刷页码；OCR 失真时回到原页，不依赖损坏公式下数学结论。
- 可复用或公开发布的技能只保存必要的公开书目信息和独立概括，不分发私人上传材料、全文或独特句式。这不限制在当前授权任务中读取、分析和编辑私人稿件。

## 2. 中文路线

中文正文优先参考中文正文，而不是英文论文的逐句译文或中文论文的英文摘要。以下结构可按当前数学依赖选择，不是强制目录：

- 适定性：模型与文献定位、解概念和工具、关键估计、主要结果及证明。模型首次出现时说明区域、变量、参数和初边值条件；定理可集中或分节陈述。
- 长期动力学：相空间与抽象判据、层级估计、吸收集、连续性或紧性、主定理中尚需验证的条件。
- 分歧与数值：平衡态和变量变换、线性谱、临界穿越、约化与分类、数值展示。数值观察不代替定理证明。

摘要用简洁的结果链说明对象与范围、关键方法和性质。存在、唯一、正则性、吸引子或分歧分类各自的适用范围应清楚；不要罗列所有初等不等式。

证明先说控制量和测试函数，再给恒等式或不等式。复杂项可命名后分别估计，合并时点明实际使用的编号及吸收、积分或 Grönwall 的作用，最后写回函数空间与结论。存在性、唯一性和正则性之间应有明确转换，不把它们混成一条无归属的估计链。

## 3. 英文路线

Use English research prose as a language reference rather than treating translated abstracts as a full-paper style model. State the object, scope, main result, and relevant mechanism clearly. Group prior work by its relationship to the current problem, and identify the specific obstruction that the selected tools address.

For a long proof, a brief roadmap and headings with mathematical purposes can help. Separate energy control, integrability, regularity improvement, compactness, passage to the limit, and uniqueness when the argument needs those distinctions. Do not fill gaps between formulas with “obviously” or “similarly.”

If modeling is part of the contribution, distinguish physical assumptions, derivation, compatibility, and PDE analysis. If the model is already given, avoid unnecessary reconstruction of the modeling section. Keep physical interpretation, proved mathematical conclusions, and methodological comparison distinct.

## 4. 比较与证据边界

- 每个观察对应可定位的段落或论证单元。说明它解决什么阅读问题、适用于什么条件，以及何时不用。
- 将单篇习惯、多篇重复做法、数学依赖所迫和编辑选择分开。多次出现不自动成为普遍规则；有限样本也不能证明中英文文体的绝对差异。
- 中文长证明同样可能需要路线说明，英文短证明也可以紧凑。章节从 0 或 1 开始等版式按目标期刊决定，不上升为论证规则。
- 不由作者顺序、共同署名、材料来源或语言相似推断私人关系、贡献分配或统一的写作制度。
- 如要求学习检验，按 [证明驱动的学习](proof-grounded-writing.md) 约定范围。风格观察本身不证明数学正确，也不证明已完成独立重建或迁移。

现有[中英文文献样本](literature-style-samples.md)可作为可选定位附录；其作者、版本、页段与风格摘要不替代本次核查，不自动成为已验证规则。[本地偏好档案](local-preferences.md)只用于选择任务相关材料，不能凌驾于当前用户要求或数学依赖。

## 按需参考入口

本索引承接精简前入口中的导航，不要求整组读取。

- 语言与全文编辑细则：[语言路线](language-routes.md)、[全文编辑](manuscript-editing.md)；只处理当前语言或交付层面。
- 证明审查需要补充清单时：[证明审查清单](proof-audit.md)。
- 具体写作范例：[PDE组织](pde-writing-style.md)、[中文PDE](chinese-pde-writing-style.md)、[椭圆与非局部](elliptic-writing-style.md)、[色散与双曲](dispersive-writing-style.md)、[抛物](parabolic-writing-style.md)；只选与当前机制相关者。
- 查来源与历史时：[证据来源](evidence-sources.md)、[文献样本](literature-style-samples.md)；书目与样本不替代当前数学核查。

## 建模与图表交付

仅在任务涉及建模验证或科研图表时采用。区分建模假设、严格推论、统计拟合与数值观察；按当前目标核对量纲、标定数据、参数可识别性、边界条件、误差来源、敏感性和验证范围。对同一数据的拟合不直接提供新数据上的验证，模拟图像不能作为数学定理的证明。

要求生成或核验图表时，保留数据来源、代码、参数、随机种子（若随机）和环境信息，实际运行后检查输出；中文图表选择环境中实际存在且支持中文的字体并验证显示，图例和坐标标明变量、量纲及必要说明。只要求审查或规划时交付对应意见，不擅自运行或出图，不伪造数据、复现记录或验证通过状态。
