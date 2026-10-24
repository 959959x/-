# 12 项任务交付

本轮仅使用指定 baseline 技能包及两份授权材料；未联网、读取其他技能版本或发表版本，未执行安装、上传、配置或技能修改。下列各项互相独立，正文后的读取与边界记录不属于拟用于论文的文字。

## 任务 1

设 Ω 为有界区域。若 u_n 在 L²(Ω) 中强收敛于 u，则 u_n⊗u_n 在 L¹(Ω) 中强收敛于 u⊗u。

读取与边界：使用 W、L、PREF；仅完成中文润色与数学表述保持，未追加证明或翻译。

## 任务 2

本文研究二维有界光滑区域 Ω 上满足齐次 Dirichlet 边界条件的模型 M。对于每个初值 u₀∈H¹₀(Ω)，我们建立全局强解的存在性与唯一性。在进一步假设 u₀∈H²(Ω)∩H¹₀(Ω) 时，对每个固定 T>0，离散解满足 sup_{0≤t≤T}‖u_h(t)−u(t)‖_{L²}≤C(T,Ω,‖u₀‖_{H²})h，其中常数与 h 无关。该估计给出有限时间区间上的一阶误差控制，但不主张常数关于 T 一致。

读取与边界：使用 W、L、PREF、FRAME；按给定结果 A、B 起草，未开展新推导，未添加文献优先权、推广关系或证明创新。

## 任务 3

For the heat equation u_t=u_xx on (0,1) with homogeneous Dirichlet boundary conditions, the supplied theorem establishes L² contractivity of the continuous solution semigroup. Separately, explicit finite-difference experiments for one smooth initial profile showed decreasing error on three grids at Δt/Δx²=0.4, while one run at 0.6 exhibited growth. These observations describe the tested computations; they establish neither a general convergence rate nor a discrete stability theorem, which remains unproved in the manuscript.

读取与边界：使用 W、L、PREF、JOURNAL；定理按所给基线表述，实验仅按提供的运行记录描述；未运行新实验或核验离散稳定性。

## 任务 4

对已合法构造的近似序列，有 ‖u_n‖_{L∞(0,T;L²)}≤C(T)，其中 C(T) 与 n 无关，但可能依赖 T；且 u_n→u 于 L²(0,T;L²) 强收敛。由于尚未核实 u 在 t=0 的时间迹，现有论证尚不足以确认全部初始条件。

读取与边界：使用 W、L、PREF；仅压缩原说明，保留初始迹缺口及常数依赖，未补证明或移置缺口。

## 任务 5

Our manuscript establishes well-posedness for model M under assumptions H and includes two sets of numerical tests. The theoretical contribution concerns the problem within the stated assumptions, while the computations provide a separate numerical component. We submit this work for consideration in Nature Communications, with the scope of the mathematical result and the numerical tests stated separately in the manuscript.

作者需要补充的事实：

- 模型 M、条件 H、适定性的准确内容及其正文位置。
- 两组数值检验的目的、设置、评价指标、实际结果和可复现材料。
- 与已有文献的具体可比关系，以及据此能够支持的贡献与期刊读者意义。
- 全体作者同意、原创性及是否同时投往其他期刊的真实情况。
- 利益冲突、资助信息，以及数据和代码是否存在、如何获取；如有仓库，提供真实链接。
- 稿件题名、作者与通讯信息、拟投文章类型。

读取与边界：使用 W、L、PREF、JOURNAL、FRAME。本轮未核对 Nature Communications 当前官方投稿规定，不能宣布格式或声明已符合要求；具体字数、必需声明和文件要求仍待核对。上文是贡献段落草稿，未声称两组实验取得了未提供的结果，亦未实际投稿。

## 任务 6

**命题。** 设 Ω 为有界区域，a_n→a，且 a_n,a≥0。若 f∈L²(Ω)，则 a_n f→af 于 L²(Ω) 强收敛。

**证明。** 由范数的齐次性，

\[
\|a_nf-af\|_{L^2(\Omega)}
=|a_n-a|\,\|f\|_{L^2(\Omega)}\longrightarrow0.
\]

故所述强收敛成立。□

阶段记录：依据用户冻结骨架完成本次隔离写作阶段的短命题及证明。未打开发表版本；后续 Mathematical Audit、Writing Audit、发表版本比较和完整训练均未执行，未宣称通过。保持全部给定假设。

读取与边界：使用 W、L、PREF、TRAIN；数学机制来自给定骨架，不声称独立发现或已完成后续复核。

## 任务 7

甲的结论不成立，不是单纯的表达省略。x_n=1−1/n 确实收敛到 1，闭性也只能帮助确认极限留在集合内；它不提供序关系上的极大性。由于 2∈[0,2] 且 2>1，1 不是该集合的极大元。建议明确保留收敛结论，并将最后一步标为错误；在不改变原命题的约束下，不能靠润色补成有效证明。

乙在所列条件下足以支持结论。建议补出承接估计：

\[
|T_nu|\ge |T_nu_n|-|T_n(u-u_n)|
\ge b_n-\|T_n\|\|u-u_n\|
\ge b_n/2.
\]

由于 T_n 非零且连续，0<‖T_n‖<∞，题中分母合法；若 b_n→∞，即得 |T_nu|→∞。这里使用的是同一个极限 u 对每个 n 的误差界。

读取与边界：使用 W、L、PREF、R、AUDIT；独立核查了上述局部推理和甲的反例。乙中序列及误差界的构造作为已给条件，未审查未提供的构造过程。

## 任务 8

这条归约中的“双射和唯一坐标”断言错误。K=[0,1]²，是二维正方形；Δ 才是位于 R⁴ 中的三维单纯形。四个顶点仿射相关，例如 a₁+a₄=a₂+a₃。具体地，

\[
A(1/2,0,0,1/2)=A(0,1/2,1/2,0)=(1/2,1/2),
\]

所以 A 不单射，也没有唯一重心坐标。A 是连续仿射满射，满射性由 K 的凸包定义给出。

**保留原像域 K。** 可以在 K×[0,1] 上直接核对所调用结果的入口：两个域是相应有限维实拓扑向量空间中的非空紧凸集，f 实值、分别连续，并具有所需的“关于 x 拟凹、关于 y 拟凸”性质。这些性质在题中已给，本例还可由 f(x,y)=x₁y 分别仿射直接看出。一般紧凸域上的结果并不要求 K 是单纯形；若所用辅助定理特别要求单纯形，则不能未经论证把正方形当作其输入。

**使用系数域 Δ。** 定义拉回函数

\[
g(\lambda,y)=f(A\lambda,y)=(\lambda_2+\lambda_4)y.
\]

需要核对 Δ 非空、紧、凸，A 的连续性、仿射性和满射性，以及 g 的全部所需性质。本例 g 分别连续、分别仿射，故固定 y 时关于 λ 拟凹，固定 λ 时关于 y 拟凸。满射性保证对每个 y，g 在 Δ 上的取值集合与 f 在 K 上的取值集合相同，因而相应上确界、下确界可回传。若得到系数域上的点 λ*，需明确取 x*=Aλ*，并利用每个 x∈K 均有原像来传回涉及所有 x 的不等式；这不需要也不产生唯一逆坐标。若进一步使用 Brouwer 或 KKM 等辅助步骤，连续自映射或全部面覆盖条件仍须针对实际构造核查。

读取与边界：使用 R、AUDIT、RULES、SION；本轮只检查给定有限凸几何接口与具体拉回函数，未读取原始论文、补称其采用某条路线或重新认证完整 Sion 定理。

## 任务 9

段落 B 更容易核查。它明确给出乘积差的拆分、L²×L²→L¹ 的 Hölder 配对以及 v_n 的有界性；而 v_n 的 L² 有界性正由其强收敛得到。因此两项估计均趋于零，结论成立。段落 A 的结论在当前假设下也是正确的，但读者须自行补出这条链。

本轮支持的一条暂时性观察是：当乘积极限的依据是本段需要读者核查的关键步骤时，写出一次差分解与匹配范数估计，可使收敛责任更清楚。它只基于这一小例子；若读者已熟悉该标准步骤且它不承担当前难点，A 的压缩写法也可能合适。不能由此推出所有证明都应展开，更不能将双强 L² 的结论照搬到双弱收敛或不匹配的指数。

读取与边界：使用 P、W、R、L、PL、PREF、LEARN、AUDIT、RULES、PRODUCT；完成给定段落的局部估计核查与表达比较。仅记单例观察，未开展其他论文阅读、迁移任务、正式训练或规则升级。

## 任务 10

In a one-dimensional elliptic boundary-value problem, u∈H¹₀(0,1) means that u and its weak derivative are square-integrable, and that u satisfies the zero boundary condition. Formally, H¹₀(0,1) is the closure, in the H¹ norm, of smooth functions supported strictly inside (0,1). In one dimension, each such u has a continuous representative whose endpoint values satisfy u(0)=u(1)=0. These endpoint values express the homogeneous Dirichlet condition, even when u is not classically differentiable.

读取与边界：使用 P、PREF、PL；仅完成给定空间的基础解释，未添加练习、研究结果或论文训练。

## 任务 11

模型 N 定义于二维有界光滑区域 Ω，并满足齐次 Dirichlet 边界条件。对每个 u₀∈H¹₀(Ω) 及固定 T>0，存在唯一强解，且 sup_{0≤t≤T}‖u(t)‖_{H¹}≤C(T,Ω,‖u₀‖_{H¹})。常数可能依赖 T；关于 T 的一致界尚未建立，吸引子的存在性亦未核验。

读取与边界：实际读取授权材料 authorized-notes.md，使用 W、L、PREF。按普通起草处理，保留给定常数依赖及未完成部分；未新增证明、文献优先权或最优性声明。

## 任务 12

这不是措辞问题，而是原推论被给定反例否定：u_n(x)=sin(nx) 在 L²(0,2π) 中弱收敛于 0，但所给计算表明 ∫₀²πu_n² dx=π，对每个 n 均不趋于 0。因此当前不能进入发表版本比较。

最小修订可写为：“u_n 在 L²(0,2π) 中弱收敛于 0，但该弱收敛本身不足以推出 ∫₀²πu_n² dx→0；对 u_n(x)=sin(nx)，该积分恒为 π。”这如实记录失败，不保留原错误断言，也不以加强假设掩盖它。

下一步应记录错误在 Writing Audit 阶段被指出这一真实次序，保持发表版本关闭，回到 Mathematical Audit：核查原断言以及所有依赖这一非线性极限的步骤，判断是否另有已给但尚未使用的有效依据；没有依据时明确记录缺口。修订并完成数学复核后，重新完成 Writing Audit，才可开启发表版本作比较。本轮仅确认这一局部反例及阶段阻塞，未宣称新发现后的整体数学复核或写作复核已通过。

读取与边界：使用 W、L、PREF、TRAIN、R、AUDIT、RULES、PRODUCT；弱收敛及积分值按题目给定事实使用，未读取发表版本或改动假设。

## 实际读取记录

所有路径均位于 `validation/`。以下是本轮真正载入正文的文件；各题的代号说明其使用关系，不表示每题重新读取一次。

材料：

- `behavior-cases.md`
- `authorized-notes.md`（任务 11 授权补充输入）

技能及引用文件：

| 代号 | 相对上述根目录的实际读取路径 |
| --- | --- |
| W | `baseline/mathematical-writing/SKILL.md` |
| R | `baseline/mathematical-reasoning/SKILL.md` |
| P | `baseline/math-paper-workflow/SKILL.md` |
| PREF | `baseline/math-paper-workflow/references/local-preferences.md` |
| L | `baseline/mathematical-writing/references/language-routes.md` |
| PL | `baseline/math-paper-workflow/references/language-routes.md` |
| FRAME | `baseline/mathematical-writing/references/research-framing.md` |
| JOURNAL | `baseline/mathematical-writing/references/journal-adaptation.md` |
| TRAIN | `baseline/mathematical-writing/references/training-contract.md` |
| AUDIT | `baseline/mathematical-reasoning/references/audit-domains.md` |
| RULES | `baseline/mathematical-reasoning/references/validated-rules.md` |
| LEARN | `baseline/math-paper-workflow/references/proof-grounded-writing.md` |
| SION | `baseline/mathematical-reasoning/references/rules/SION-M03.md` |
| PRODUCT | `baseline/mathematical-reasoning/references/rules/MR-O001.md` |

另外仅枚举过 baseline 目录的文件路径，未打开未列入上表的文件正文。TRAIN 的首次批量工具展示被截断，随后单独完整读取；没有将截断展示冒充完整阅读。未读取历史 Evidence、其他评测结果或其他会话；本交付不评价技能，不代表完成论文级数学审查、期刊规则核验或完整训练。
