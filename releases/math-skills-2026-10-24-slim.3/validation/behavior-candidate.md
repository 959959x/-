# 12 项任务交付

本轮仅使用指定原始材料、任务 11 的授权补充材料及 `math-skills-2026-10-24-slim.3` 内下列文件。未联网、未读取发表版本、其他版本或测试结果，未执行提交、上传、安装、配置修改或技能修改。各项相互独立；文末列出实际载入路径，以下以文件代号标注。

## 任务 1

设 Ω 为有界区域。若 u_n 在 L²(Ω) 中强收敛于 u，则 u_n⊗u_n 在 L¹(Ω) 中强收敛于 u⊗u。

使用文件：W、L。边界：仅润色中文，未补写证明或开展独立证明审查。

## 任务 2

本文研究二维有界光滑区域 Ω 上具有齐次 Dirichlet 边界条件的模型 M。首先，对每个初值 u₀∈H¹₀(Ω)，建立唯一全局强解的存在性。进一步，当 u₀∈H²(Ω)∩H¹₀(Ω) 时，对任意固定 T>0，离散解满足误差估计 sup_{0≤t≤T}‖u_h(t)−u(t)‖_{L²}≤C(T,Ω,‖u₀‖_{H²})h，其中 C 与 h 无关。该估计给出有限时间区间上的一阶误差控制，常数允许依赖 T，不包含关于 T 的一致结论。

使用文件：W、L、FR、J。边界：按给定结果起草，未新增推导、文献优先权或证明创新声明；未独立验证模型 M 的定理。

## 任务 3

For the heat equation u_t=u_xx on (0,1) with homogeneous Dirichlet boundary conditions, the supplied theorem establishes L² contractivity of the continuous solution semigroup. Separately, an explicit finite-difference experiment with Δt/Δx²=0.4 showed decreasing error across three grids for one smooth initial profile, whereas growth was observed in one run at Δt/Δx²=0.6. These observations concern only the reported runs: they do not establish a convergence rate or a general discrete stability result, and the manuscript has not proved a discrete stability theorem.

使用文件：W、L、J。边界：未重算实验，也未把连续半群的收缩性传给离散格式。

## 任务 4

对已合法构造的近似序列，有 ‖u_n‖_{L∞(0,T;L²)}≤C(T)，其中常数与 n 无关，但可能依赖 T；同时，u_n 在 L²(0,T;L²) 中强收敛于 u。由于尚未核实 u 在 t=0 的时间迹，目前不能宣称已建立全部初始条件。

使用文件：W、L、VW。边界：压缩给定说明，保留初始迹缺口；未新增极限或迹的证明。

## 任务 5

Our manuscript establishes well-posedness for model M under assumptions H and reports two sets of numerical tests. The analytical contribution is the well-posedness result within these assumptions; the numerical tests provide computational observations within the configurations studied. Their specific findings and relationship to the theoretical result should be stated once the corresponding details are supplied.

作者需要补充或确认的事实：

- 模型 M、条件 H、适定性结论的具体范围，以及与可比已有文献的关系。
- 两组数值检验的设置、指标和结果，及其与理论结论的实际联系。
- 题名、作者与通讯作者信息、全体作者同意投稿的确认，以及原创性和投稿状态。
- 利益冲突、资助、数据与代码的实际可用性、仓库或访问方式；不存在相应材料时也应据实说明。

本轮无法联网，因此没有核对 Nature Communications 当前官方投稿指南、文章类型或声明要求；上述清单是草稿所缺事实，不表示这些项目已满足该刊现行规定。正式投稿前仍需核对适用指南。

使用文件：W、L、FR、J。边界：仅贡献段落及缺失事实清单，未核文献、期刊现行规则或作者声明，未提交投稿。

## 任务 6

**命题。** 设 Ω 为有界区域，a_n→a 且 a_n,a≥0。若 f∈L²(Ω)，则 a_n f→af 于 L²(Ω)。

**证明。** 由范数的齐次性，

\[
\|a_n f-af\|_{L^2(\Omega)}
=|a_n-a|\,\|f\|_{L^2(\Omega)}\longrightarrow0.
\]

故结论成立。

阶段记录：本次完成给定冻结骨架下的第 3 阶段 Write independently（隔离独立写作）。未打开发表版本，未完成后续 Mathematical Audit、Writing Audit、发表版本比较或完整训练；此稿不作为这些阶段已经通过的记录。

使用文件：W、L、T。边界：沿用给定条件和机制，没有增加数学基线；本记录只覆盖本次短命题的写作阶段。

## 任务 7

**甲的结论错误，不能靠润色补成。** 由 x_n=1−1/n 可知 x_n→1，而闭性只保证极限仍属于 [0,2]，不保证极大性。由于 2∈[0,2] 且 2>1，1 不是该集合在通常次序下的极大元。建议保留收敛结论并明确标注后续极大性断言不成立；若仍要求原结论，其所需的“无严格后继”性质已被 2 否定，不能默认为已证明。

**乙的条件足以支持结论。** 建议补出一行定量估计，使余量如何保留可以直接核查：

\[
|T_nu|\ge |T_nu_n|-|T_n(u-u_n)|
\ge b_n-\|T_n\|\,\|u-u_n\|
\ge b_n/2.
\]

非零连续线性泛函保证 0<‖T_n‖<∞，所给误差界有意义。若 b_n→∞，上述下界即给出 |T_nu|→∞。这里已有足够的定量误差控制，无需另设缺失的尾部论证。

使用文件：W、R、L、VW。边界：实际核查了两段局部推理；未更改其假设或将甲替换成另一命题，也未审查 u_n 的外部构造过程。

## 任务 8

原归约不成立。K=[0,1]² 是二维正方形；Δ 是 R⁴ 中的三维标准单纯形。A 是连续仿射满射，但不是单射。例如

\[
A(1/2,0,0,1/2)=A(0,1/2,1/2,0)=(1/2,1/2).
\]

这也对应仿射依赖 a₁+a₄=a₂+a₃。因此不能声称 K 是三维单纯形或每点具有唯一重心坐标。

**保留 K。** 在 R² 的通常拓扑上，K 本身就是合法的有限维紧凸域。给定的非空、紧凸、实值、分别连续及“对 x 拟凹、对 y 拟凸”条件应与拟用极小极大命题的变量方向和全部假设逐项对应。本例 f(x,y)=x₁y 对每个变量均为仿射函数，所给函数性质可以直接核实。若中间步骤调用 Brouwer，仍须构造并核验相应的连续自映射；若调用要求单纯形的覆盖定理，则须另核单纯形结构及全部面条件，不能因 K 有有限生成点就跳过。

**使用 Δ。** 取拉回函数

\[
F(\lambda,y)=f(A\lambda,y)=(\lambda_2+\lambda_4)y.
\]

须核 Δ 的非空、紧凸性、A 的连续仿射性与满射性，以及 F 的函数性质。本例 F 实值、连续且分别仿射，因此对 λ 拟凹、对 y 拟凸；一般情况下，相应水平集的凸性也可由仿射原像检查。若继续使用固定点或覆盖工具，仍须核该工具的映射或面条件。最后必须回传结论：由 A(Δ)=K，遍历 λ 与遍历 x 得到相同的函数值范围；若在 Δ×[0,1] 得到鞍点 (λ*,y*)，则其不等式可借满射性传回 (Aλ*,y*)。这些步骤不需要唯一重心坐标，也没有提供连续逆坐标。

使用文件：R、L、VR、SC。边界：本轮检查的是所给方形、参数化和函数接口；未读取原始论文、补造其证明细节或重新认证整篇 Sion 定理。

## 任务 9

段落 B 更便于直接核查：它明确给出乘积差的拆分、Hölder 不等式及 ‖v_n‖₂ 有界这一输入。后者由 v_n→v 于 L²(Q) 得到，因此右侧两项确实趋于零。段落 A 的结论在本题条件下正确，但读者需要自行恢复这条推理，或找到此前已证明的乘积极限结论。

本轮可支持的一条暂时观察是：**当乘积极限是当前需要核查的步骤时，给出一行显示趋零因子与有界因子的估计，有助于读者定位结论依据。** 这一观察只来自本例；若该接口已在前文证明，或读者可直接调用已有结果，简写也可以充分。不能据此推成“越详细越好”，也不能外推到弱弱收敛或不匹配指数的乘积。

使用文件：F、R、W、L、P、VW、VR、MC。边界：仅核查并比较这两段；没有其它论文证据、读者实验或后续迁移检验，未形成已验证的普遍写作规则，未继续选材、保存技能或上传。

## 任务 10

In a one-dimensional elliptic boundary-value problem, u∈H¹₀(0,1) means that u and its weak first derivative (a generalized derivative) are square-integrable on (0,1), and u satisfies the zero boundary condition at both endpoints. In one dimension, such a function has a continuous representative, so this condition can be written as u(0)=u(1)=0. Formally, H¹₀ is the closure of smooth functions supported strictly inside the interval in the H¹ norm; the subscript 0 refers to the boundary values, not to u being zero everywhere.

使用文件：F、R、L。边界：仅作所请求的基础概念解释，未求解具体椭圆方程或启动论文训练。

## 任务 11

对二维有界光滑区域 Ω 上施加齐次 Dirichlet 边界条件的模型 N，若 u₀∈H¹₀(Ω)，则对每个固定 T>0 存在唯一强解，且 sup_{0≤t≤T}‖u(t)‖_{H¹}≤C(T,Ω,‖u₀‖_{H¹})。常数可依赖 T；关于 T 的一致界尚未建立，吸引子存在性尚未核验。

使用文件：W、L、N（已实际读取授权补充材料）。边界：普通起草，未开展新证明，未添加优先权、最优性或吸引子存在的声明。

## 任务 12

该写法包含数学错误：弱 L² 收敛不足以推出平方积分趋于零。给定的 u_n(x)=sin(nx) 已弱收敛于零，但

\[
\int_0^{2\pi}u_n(x)^2\,dx=\pi\ne0,
\]

直接否定原推论。这不是连接词或措辞问题，不能把“弱收敛”暗改为“强收敛”来保留原断言。

**当前不能进入发表版本比较。** 应记录错误是在 Writing Audit 中发现，回到 Mathematical Audit，检查这一错误影响了哪些下游估计和结论；按原假设撤回不成立的推论，明确哪些目标仍无证明。完成必要修正与数学复核后，重新进行 Writing Audit，两项门槛通过后才进入发表版本比较。

这也符合本轮读取的[训练契约](../mathematical-writing/references/training-contract.md)原文：“若发现数学错误，记录真实发现次序，暂停来源比较，修正并回到 Mathematical Audit；复核通过后重新完成 Writing Audit。”

使用文件：W、R、L、T、VR、MC。边界：本轮确认了该局部推论被给定反例否定；没有完成新发现后的全部数学复核或重新写作审查，未打开发表版本，未改变原假设。

## 实际载入文件记录

以下均位于 `WORKSPACE/`。代码用于缩短逐项记录；每行给出实际文件路径，不代表载入了其链接指向的所有文件。

| 代号 | 实际路径（相对于上述绝对根目录） |
|---|---|
| 原始材料 | `output/math-skills-2026-10-24-slim.3/behavior-cases.md` |
| N | `output/math-skills-2026-10-24-slim.3/authorized-notes.md` |
| W | `math-skills-2026-10-24-slim.3/mathematical-writing/SKILL.md` |
| R | `math-skills-2026-10-24-slim.3/mathematical-reasoning/SKILL.md` |
| F | `math-skills-2026-10-24-slim.3/math-paper-workflow/SKILL.md` |
| L | `math-skills-2026-10-24-slim.3/math-paper-workflow/references/local-preferences.md` |
| FR | `math-skills-2026-10-24-slim.3/mathematical-writing/references/research-framing.md` |
| J | `math-skills-2026-10-24-slim.3/mathematical-writing/references/journal-adaptation.md` |
| VW | `math-skills-2026-10-24-slim.3/mathematical-writing/references/validated-rules.md` |
| T | `math-skills-2026-10-24-slim.3/mathematical-writing/references/training-contract.md` |
| P | `math-skills-2026-10-24-slim.3/math-paper-workflow/references/proof-grounded-writing.md` |
| VR | `math-skills-2026-10-24-slim.3/mathematical-reasoning/references/validated-rules.md` |
| SC | `math-skills-2026-10-24-slim.3/mathematical-reasoning/references/rules/SION-M03.md` |
| MC | `math-skills-2026-10-24-slim.3/mathematical-reasoning/references/rules/MR-O001.md` |

实际技能版本范围为目录 `math-skills-2026-10-24-slim.3`。首次批量返回有截断，因此另行完整读取了 VW 与 T。未打开任何来源证据文件、候选规则库、技能版本说明或链接中的外部论文；引用技能中列出的历史标签不构成本轮对其历史证据的独立验证。
