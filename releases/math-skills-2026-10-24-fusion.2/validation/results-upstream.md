# 9项独立请求交付

使用材料：本目录的 `behavior-cases.md`，以及分配的 `upstream/` 内三个技能及下列实际读取的引用文件。各项答案独立；未联网，未执行上传、安装、配置修改或技能修改。未读取其它技能版本、其它测试结果或历史对话记录。

## 任务1

设 \(\Omega\) 为有界区域。若 \(u_n\) 在 \(L^2(\Omega)\) 中强收敛于 \(u\)，则 \(u_n\otimes u_n\) 在 \(L^1(\Omega)\) 中强收敛于 \(u\otimes u\)。

## 任务2

本文研究模型 \(M\) 的全局强解及其离散近似。在二维有界光滑区域 \(\Omega\) 上，施加齐次 Dirichlet 边界条件，对任意 \(u_0\in H_0^1(\Omega)\)，证明全局强解的存在唯一性。若进一步有 \(u_0\in H^2(\Omega)\cap H_0^1(\Omega)\)，则对每个 \(T>0\)，离散解满足
\[
\sup_{0\le t\le T}\|u_h(t)-u(t)\|_{L^2}
\le C(T,\Omega,\|u_0\|_{H^2})h,
\]
其中 \(C\) 与 \(h\) 无关。因此，该误差估计给出有限时间区间上的一阶收敛；常数允许依赖 \(T\)，不主张对时间一致。

## 任务3

The supplied theorem establishes \(L^2\) contractivity of the solution semigroup for the heat equation \(u_t=u_{xx}\) on \((0,1)\) with homogeneous Dirichlet boundary conditions. In the explicit finite-difference experiment, the error decreased across three grids for one smooth initial profile at \(\Delta t/\Delta x^2=0.4\), whereas one run at \(0.6\) exhibited growth. These observations concern the reported computations; they neither establish a general convergence rate nor prove discrete stability. In particular, the manuscript has not proved a discrete stability theorem, and the continuous contractivity result does not by itself provide one.

## 任务4

对已合法构造的近似序列，有
\[
\|u_n\|_{L^\infty(0,T;L^2)}\le C(T),
\]
其中常数与 \(n\) 无关，但可依赖 \(T\)；且 \(u_n\) 在 \(L^2(0,T;L^2)\) 中强收敛于 \(u\)。由于尚未核实 \(u\) 在 \(t=0\) 的时间迹，目前不能宣称全部初始条件已建立。

## 任务5

**Cover letter贡献段落**

Our manuscript establishes well-posedness for model \(M\) under assumptions \(H\) and presents two sets of numerical tests. The theoretical result is confined to the setting specified by \(H\), while the numerical component concerns the two reported test configurations.

**作者需补充的事实**

- 模型 \(M\)、条件 \(H\) 及适定性结论的准确范围；稿件题名、作者及通讯作者信息。
- 与已有文献的具体比较，以及据此能够支持的贡献定位和对 Nature Communications 读者的相关性。
- 两组数值检验的目的、设置、主要结果和可复现信息。
- 全体作者是否同意投稿，以及需披露的利益冲突事实。
- 数据与代码是否可获得、仓库或访问路径，以及存在的限制及其原因。
- 首次投稿需要说明的稿件状态及相关事实，并在核查现行要求后补全相应声明。

本轮未联网，未核查 Nature Communications 的现行投稿规定。以上是依据所给材料起草的贡献说明和事实补充清单，不代表稿件已满足该刊全部要求。

## 任务6

**命题。** 设 \(\Omega\) 为有界区域，\(a_n\to a\)，其中 \(a_n,a\ge0\)，且 \(f\in L^2(\Omega)\)。则 \(a_nf\to af\) 于 \(L^2(\Omega)\) 中强收敛。

**证明。** 由范数的齐次性，
\[
\|a_nf-af\|_{L^2(\Omega)}
=|a_n-a|\,\|f\|_{L^2(\Omega)}
\longrightarrow0.
\]
故结论成立。 \(\square\)

阶段记录：依据所给冻结骨架完成了本单元的独立写作，停在训练流程的 Write independently 阶段。未打开发表版本，未执行后续 Mathematical Audit、Writing Audit、来源比较或迁移检验，也未完成整轮训练。

## 任务7

**甲：原结论不成立，不能靠表达润色补足。** 由给定公式确有 \(x_n\to1\in[0,2]\)，但 \(2\in[0,2]\) 且 \(2>1\)，所以 \(1\) 不是该集合在通常次序下的极大元。递增、Cauchy 及闭性只支持相应的收敛和极限属于集合，不能排除集合中更大的元素。建议保留已支持的收敛说明，并明确标出最后一步错误；在不改变命题的范围内，不能将这段证明改写为已完成的极大元证明。

**乙：给定条件足以支持所写推论。** 建议补出误差控制的一行：
\[
|T_nu|
\ge |T_nu_n|-|T_n(u-u_n)|
\ge b_n-\|T_n\|\,\|u-u_n\|
\ge b_n/2.
\]
因此，若 \(b_n\to\infty\)，则 \(|T_nu|\to\infty\)。这里使用的是每个 \(T_n\) 的连续性及逐项给定的误差界，不需要另设 \(\sup_n\|T_n\|<\infty\)。本次核查了从给定条件到该结论的推理；题目所称 \(u_n\) 及其误差界的构造过程未提供，未核查该构造。

## 任务8

这条归约中的几何断言不成立。此处 \(K=[0,1]^2\)，是二维正方形；\(\Delta\) 才是三维单纯形。映射
\[
A(\lambda)=(\lambda_2+\lambda_4,\lambda_3+\lambda_4)
\]
连续、仿射且满射，但不是单射。例如
\[
A(1/2,0,0,1/2)=A(0,1/2,1/2,0)=(1/2,1/2).
\]
所以不能主张唯一重心坐标或双射。

**保留 \(K\) 的做法。** \(K\) 已是 \(\mathbb R^2\) 中的非空紧凸集；另一个域为非空紧凸集 \([0,1]\)。给定的实值性、分别连续性及关于 \(x\) 拟凹、关于 \(y\) 拟凸的方向，应与实际拟用的极小极大结论逐项对应。本例 \(f(x,y)=x_1y\) 在固定任一变量后都是仿射函数，这些函数性质可直接核查。若证明进一步调用 Brouwer，则仍须给出相应紧凸域上的连续自映射；若调用只针对单纯形的 KKM 形式，则不能把正方形直接当作该形式所需的单纯形，仍须说明合法接口并核查覆盖及面条件。

**使用 \(\Delta\) 的做法。** 定义
\[
g(\lambda,y)=f(A(\lambda),y)=(\lambda_2+\lambda_4)y.
\]
需核查 \(\Delta\) 的非空、紧、凸性质，\(A\) 的连续仿射性及满射性，以及拉回函数的性质。本例 \(g\) 实值、分别连续，对固定 \(y\) 关于 \(\lambda\) 仿射，故拟凹；对固定 \(\lambda\) 关于 \(y\) 仿射，故拟凸。一般而言，这里拟凹性的传递可由凸超水平集在仿射映射下的原像仍凸来核查。改用系数域不免除后续连续自映射或覆盖面条件等责任。

最终还须把辅助结论送回原域。满射性保证每个 \(x\in K\) 都有系数表示，因而固定 \(y\) 时，遍历 \(\lambda\in\Delta\) 与遍历 \(x\in K\) 得到相同的函数值集合。若已在系数域证明相应鞍点不等式，令 \(x_*=A(\lambda_*)\)，并对任意 \(x\) 选择一个原像，即可传回原域；这一方向不需要唯一坐标或连续逆映射。

本轮核查的是给定例子的几何、函数拉回及回传责任；未读取原始论文，未补造原论文证明细节，也未重新认证整篇 Sion 定理。

## 任务9

段落B更容易核查：它展示了乘积差的分解、Hölder 不等式的配对指数，以及 \(v_n\) 的 \(L^2(Q)\) 有界性如何参与闭合。该有界性由 \(v_n\to v\) 于 \(L^2(Q)\) 直接得到，例如 \(\|v_n\|_2\le\|v_n-v\|_2+\|v\|_2\)。因此，B中估计右端的两项均趋于零，结论成立。段落A的结论在给定条件下也成立，但读者须自行恢复这些步骤。

本轮可支持的一条暂时性观察是：**当乘积收敛是当前论证中需要核查的一步时，写出差的分解，并指出趋零因子及有界因子，有助于读者看清输入怎样推出目标范数收敛。** 这里的证据仅是这一个 \(L^2(Q)\times L^2(Q)\to L^1(Q)\) 小例子，属于局部观察，不能升级为跨论文规则。若前文已明确给出适用引理，或目标读者无需重复该标准步骤，A式简写也可能合适；不能据此要求所有证明都展开。数学结论也不能直接迁移到弱—弱收敛、不同积分指数或仅局部收敛却要求整体范数收敛的情形。

本轮完成了所给两段的局部估计核查和表达比较；未执行其它论文阅读、后续迁移任务或技能更新。

## 实际读取记录

以下均为实际读取路径。除任务材料外，读取范围仅在指定的 `upstream/` 三个目录中。长文件 `validated-rules.md` 的首次整文件工具输出出现截断，随后另外读取了 MR-O001、MR-O002 和 SION-M03 的完整段落；不将未显示部分记为完整阅读。

| 编号 | 实际读取的绝对路径 | 本轮用途 |
|---|---|---|
| C1 | `validation/behavior-cases.md` | 任务1—9的原始请求与给定材料 |
| W1 | `upstream/mathematical-writing/SKILL.md` | 任务1—7的写作、润色、范围与审查分流 |
| W2 | `upstream/mathematical-writing/references/language-routes.md` | 任务1—7的语言保持与原创写作路线 |
| W3 | `upstream/mathematical-writing/references/training-contract.md` | 任务6的隔离写作与阶段记录；任务9的受限练习边界 |
| R1 | `upstream/mathematical-reasoning/SKILL.md` | 任务7—8的数学审查与未核边界 |
| R2 | `upstream/mathematical-reasoning/references/audit-domains.md` | 任务7—8的条件、反例与证明缺口区分 |
| R3 | `upstream/mathematical-reasoning/references/validated-rules.md` | MR-O001用于任务9的乘积配对；MR-O002核对算子检查适用范围；SION-M03用于任务8的有限凸几何接口 |
| P1 | `upstream/math-paper-workflow/SKILL.md` | 任务9的限定学习范围 |
| P2 | `upstream/math-paper-workflow/references/language-routes.md` | 任务9的中文表达 |
| P3 | `upstream/math-paper-workflow/references/proof-grounded-writing.md` | 任务9的局部理解、比较与观察边界 |

技能内已有的历史证据摘要仅按其公开文本读取，未读取其提及的原论文或历史支持记录，也不将这些摘要记作本轮重新核验。当前任务未提供全文、原始实验数据、期刊现行要求或完整构造；未声称完成这些验证。
