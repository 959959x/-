# 基线技能使用交付

日期：2026-10-24。输入为 `behavior-cases.md` 中的任务 1—9，所用技能版本为同目录 `baseline/` 包。本轮只交付这些任务，不评价或修改技能。下列 R 编号对应文末实际读取路径；文件只读取一次时，不重复计作阅读。

## 任务 1

设 \(\Omega\) 为有界区域。若 \(u_n\) 在 \(L^2(\Omega)\) 中强收敛于 \(u\)，则 \(u_n\otimes u_n\) 在 \(L^1(\Omega)\) 中强收敛于 \(u\otimes u\)。

读取：R1、R4。仅完成中文润色，未补写证明。

## 任务 2

本文研究二维有界光滑区域 \(\Omega\) 上具有齐次 Dirichlet 边界条件的模型 \(M\)。对于每个 \(u_0\in H^1_0(\Omega)\)，本文证明全局强解存在且唯一。进一步，若 \(u_0\in H^2(\Omega)\cap H^1_0(\Omega)\)，则对每个固定 \(T>0\)，离散解满足
\[
\sup_{0\le t\le T}\|u_h(t)-u(t)\|_{L^2}
\le C(T,\Omega,\|u_0\|_{H^2})h.
\]
常数 \(C\) 与 \(h\) 无关，但允许依赖 \(T\)。上述结果给出了相应初值类中的全局强解结论，以及更高正则初值下的有限时间一阶误差控制；这里不主张误差界对 \(T\) 一致。

读取：R1、R4、R5。依据给定数学基线起草，未独立核验定理或开展文献比较。

## 任务 3

The supplied theorem establishes \(L^2\) contractivity of the solution semigroup for the heat equation on \((0,1)\) with homogeneous Dirichlet boundary conditions. In the explicit finite-difference experiments, the error decreased across three grids at \(\Delta t/\Delta x^2=0.4\) for one smooth initial profile, whereas one run at a ratio of \(0.6\) exhibited growth. These observations are limited to the tested settings and do not establish a general discrete stability or convergence result; the manuscript contains no proof of discrete stability.

读取：R1、R4、R6。仅区分给定连续理论与数值观察，未运行数值实验或新增离散定理。

## 任务 4

对已合法建立的近似序列，有
\[
\|u_n\|_{L^\infty(0,T;L^2)}\le C(T),
\qquad u_n\to u\quad\text{于 }L^2(0,T;L^2)\text{ 强收敛},
\]
其中 \(C(T)\) 与 \(n\) 无关，但可能依赖 \(T\)。由于尚未核实 \(u\) 在 \(t=0\) 的时间迹，不能据此宣称全部初始条件已经成立。

读取：R1、R4、R6。保留原有条件与初始迹缺口，未新增证明或移入附录。

## 任务 5

Our manuscript establishes well-posedness for model \(M\) under assumptions \(H\) and presents two sets of numerical tests. The theoretical claim is restricted to the regime specified by \(H\), while the computations provide observations within the tested settings. The contribution statement should be supplemented with a verified comparison to existing results before making claims of novelty or broader significance.

作者需要补充的事实：

- 模型 \(M\)、条件 \(H\)、解类及适定性结论的准确范围，以及可核实的已有文献对照。
- 两组数值检验的目的、方法、参数、结果和可复现材料。
- 全体作者是否同意投稿、利益冲突情况；其他原创性或投稿状态声明也须由作者确认。
- 实际使用或产生的数据与代码、可用性及访问方式；如有仓库，提供真实链接及访问限制。
- 稿件题名、作者和通讯作者信息，以及拟投文章类型。

本轮未联网，未核对 Nature Communications 当前官方投稿指南、投稿信格式或声明要求；以上是基于已给事实的贡献草稿与补充清单，不代表已符合期刊要求。

读取：R1、R4、R5、R6。未提交、上传或联系期刊。

## 任务 6

**命题。** 设 \(\Omega\) 为有界区域，\(a_n\to a\)，且 \(a_n,a\ge0\)。若 \(f\in L^2(\Omega)\)，则 \(a_nf\to af\) 于 \(L^2(\Omega)\) 强收敛。

**证明。** 由范数的齐次性，
\[
\|a_nf-af\|_{L^2(\Omega)}
=|a_n-a|\,\|f\|_{L^2(\Omega)}\longrightarrow0.
\]
结论成立。

阶段记录：依据题目提供的冻结骨架完成本次“隔离写作”阶段。未打开发表版本，未实施后续 Mathematical Audit、Writing Audit、来源比较或迁移验证，也不声称整项训练已完成；此前阶段视为用户提供的输入状态，未追认本轮完成。

读取：R1、R4、R7。

## 任务 7

**甲不能支持结论，且结论本身为假。** \(x_n\to1\) 成立，但闭性至多用于确认极限仍属于集合，不能推出极大性。因为 \(2\in[0,2]\) 且 \(2>1\)，所以 \(1\) 不是极大元。修改建议：明确指出从“极限在集合中”到“极大元”的推理无效；在保持原命题的要求下，无法仅靠润色修复此证明。

**乙在给定条件下成立。** 建议将关键估计写全：
\[
|T_nu|\ge |T_nu_n|-|T_n(u-u_n)|
\ge b_n-\|T_n\|\,\|u-u_n\|
\ge \frac{b_n}{2}.
\]
这里连续性给出算子范数估计，\(T_n\ne0\) 保证分母为正。若 \(b_n\to\infty\)，则同一个 \(u\) 满足 \(|T_nu|\to\infty\)。这一步不需要 \(\|T_n\|\) 一致有界；已给误差估计已逐项控制 \(T_n\) 的放大作用。

读取：R1、R2、R4、R8、R9。核查范围仅限题给两段，不推定未提供的构造过程已获证明。

## 任务 8

该归约的理由不成立。\(K=[0,1]^2\) 是二维正方形；四个生成点不仿射独立，因为 \(a_1+a_4=a_2+a_3\)。\(\Delta\) 才是三维标准单纯形，而
\[
A(\lambda)=(\lambda_2+\lambda_4,\lambda_3+\lambda_4)
\]
是连续仿射满射，并非双射。例如
\[
A(1/2,0,0,1/2)=A(0,1/2,1/2,0)=(1/2,1/2),
\]
所以凸组合表示不唯一。

**保留 \(K\)。** 不必把凸域换成单纯形。若采用在 \(x\) 上取上确界、在 \(y\) 上取下确界的极小极大形式，应核对所调用版本要求的凸性、紧性、实值性，以及关于 \(x\) 的上半连续和拟凹、关于 \(y\) 的下半连续和拟凸。题给两域非空、紧且凸，分别连续提供所需半连续性，给定的拟凹、拟凸方向也相符；就本例而言，\(f(x,y)=x_1y\) 对每个变量分别仿射。

**使用 \(\Delta\)。** 定义拉回函数
\[
F(\lambda,y)=f(A\lambda,y)=(\lambda_2+\lambda_4)y.
\]
仍须核查 \(\Delta\) 非空、紧且凸，以及 \(F\) 的相应函数性质。本例 \(F\) 连续、分别仿射，因而满足要求。一般地，固定 \(y\) 时拟凹函数的上水平集在仿射映射下的原像仍凸；固定 \(\lambda\) 时，\(F(\lambda,\cdot)=f(A\lambda,\cdot)\)，可继承相应拟凸性。由 \(A(\Delta)=K\)，
\[
\sup_{\lambda\in\Delta}\inf_{y\in[0,1]}F(\lambda,y)
=\sup_{x\in K}\inf_{y\in[0,1]}f(x,y),
\]
且对每个 \(y\)，\(\sup_{\lambda\in\Delta}F(\lambda,y)=\sup_{x\in K}f(x,y)\)，故另一个极小极大表达式也保持。这里用到满射与拉回定义，不要求重心坐标唯一；若换用另一个 \(\Delta\) 上的函数，则不能跳过其性质及是否沿 \(A\) 的纤维取相同值的核查。

读取：R2、R8、R9。以上只核查题给有限凸几何映射及本例函数的归约条件，未读取原始论文，也未重新认证整篇 Sion 定理。

## 任务 9

段落 B 更容易核查。它写明乘积差的分解、Hölder 不等式及 \(v_n\) 的 \(L^2\) 有界性；后者由 \(v_n\to v\) 强收敛得到。因此第一项是趋零因子乘有界因子，第二项由 \(v_n-v\to0\) 和固定的 \(\|u\|_2<\infty\) 趋零。段落 A 的结论在给定条件下正确，但省略了这些可检查的依赖。

本轮支持的一条暂时性观察是：在同一域上处理两个 \(L^2\) 强收敛因子的乘积时，写出一次差分解及范数估计，能让读者直接核对目标空间和各因子的责任。该观察只基于此例，不足以成为普遍写作规则。若相同估计刚在前文建立，简短引用可能更合适；弱弱收敛、指数不匹配或不同域上的结论均须另行核查，不能照搬。本轮未进行其他论文比较或迁移测试。

读取：R3、R1、R2、R4、R9、R10。仅完成限定比较与暂时性观察，未选新论文、保存技能或上传。

## 实际读取路径

任务材料：

- `validation/behavior-cases.md`

技能与引用文件：

- R1：`baseline/mathematical-writing/SKILL.md`
- R2：`baseline/mathematical-reasoning/SKILL.md`
- R3：`baseline/math-paper-workflow/SKILL.md`
- R4：`baseline/mathematical-writing/references/language-routes.md`
- R5：`baseline/mathematical-writing/references/research-framing.md`
- R6：`baseline/mathematical-writing/references/journal-adaptation.md`
- R7：`baseline/mathematical-writing/references/training-contract.md`
- R8：`baseline/mathematical-reasoning/references/audit-domains.md`
- R9：`baseline/mathematical-reasoning/references/validated-rules.md`
- R10：`baseline/math-paper-workflow/references/proof-grounded-writing.md`

读取说明：所有上述文件均实际读取。首次批量工具输出有截断，随后单独重读 R7、R8、R9；未将参考文件中的文献摘要当作本轮已经阅读或核验原论文的记录。除题给材料与此基线包所列文件外，未读取其他技能版本、评估意见、其他测试结果或历史对话；未联网、安装、改配置或修改技能。报告完成后仅核查本报告的保存状态与任务编号。
