# 九项任务交付

本轮仅使用指定融合技能包与任务材料；以下各项独立作答。未联网，未运行所述数值实验，未核验当前期刊规定或任何原始论文；未读取其他版本或测试结果，未修改技能，未上传、安装或更改配置。

## 任务1

设 \(\Omega\) 为有界区域。若 \(u_n\) 在 \(L^2(\Omega)\) 中强收敛于 \(u\)，则 \(u_n\otimes u_n\) 在 \(L^1(\Omega)\) 中强收敛于 \(u\otimes u\)。

## 任务2

本文研究二维有界光滑区域 \(\Omega\) 上具有齐次 Dirichlet 边界条件的模型 M。对于每个 \(u_0\in H_0^1(\Omega)\)，建立全局强解的存在唯一性。若进一步假设 \(u_0\in H^2(\Omega)\cap H_0^1(\Omega)\)，则对任意固定的 \(T>0\)，离散解满足 \(\sup_{0\le t\le T}\|u_h(t)-u(t)\|_{L^2}\le C(T,\Omega,\|u_0\|_{H^2})h\)，其中常数 \(C\) 与 \(h\) 无关。这一估计给出有限时间区间上的 \(L^2\) 一阶误差控制，不包含关于 \(T\) 的一致性结论。

## 任务3

For the heat equation \(u_t=u_{xx}\) on \((0,1)\) with homogeneous Dirichlet boundary conditions, the supplied theorem establishes \(L^2\) contractivity of the continuous solution semigroup. Separately, an explicit finite-difference experiment for one smooth initial profile showed decreasing error across three grids at \(\Delta t/\Delta x^2=0.4\), whereas one run at \(0.6\) exhibited growth. These observations concern only the reported runs: they neither establish a discrete stability theorem nor determine a general stability threshold, and continuous contractivity alone does not provide either conclusion for the discretization.

## 任务4

对已合法构造的近似序列，有 \(\|u_n\|_{L^\infty(0,T;L^2)}\le C(T)\)，其中常数与 \(n\) 无关但可依赖 \(T\)，且 \(u_n\to u\) 于 \(L^2(0,T;L^2)\) 强收敛。尚未核实 \(u\) 在 \(t=0\) 的时间迹，故不能据此宣称已建立全部初始条件。

## 任务5

The manuscript establishes well-posedness for model M under assumptions H and includes two sets of numerical tests. The well-posedness theorem constitutes the analytical contribution, while the computations are limited to the settings actually tested.

作者需补充或确认的事实：

- 模型 M、条件 H、适定性所用解类及结果的准确范围。
- 可核对的已有文献比较，以及据此能够支持的贡献定位。
- 两组数值检验的设置、指标、结果及可复现材料。
- 论文题名、作者与通讯作者信息、全体作者同意投稿的真实情况。
- 利益冲突、资助，以及原创性和是否同时投往其他期刊等实际状态。
- 数据和代码是否存在、能否获取；如有仓库，提供真实链接，如无，则说明实际情况。

本轮只起草贡献说明并核对其与给定材料的对应关系。由于不能联网，未核验 Nature Communications 当前的投稿信、声明及数据/代码政策；上述清单也不冒充期刊的现行必交清单，尚不能宣布已符合投稿要求。

## 任务6

**命题。** 设 \(\Omega\) 有界，\(a_n,a\ge0\) 且 \(a_n\to a\)。若 \(f\in L^2(\Omega)\)，则 \(a_nf\to af\) 于 \(L^2(\Omega)\)。

**证明。** 由范数的齐次性，

\[
\|a_nf-af\|_{L^2(\Omega)}
=|a_n-a|\,\|f\|_{L^2(\Omega)}\longrightarrow0.
\]

故结论成立。

阶段记录：本轮依据用户已冻结的数学骨架完成第 3 阶段“独立写作”，没有打开发表版本。前置骨架作为给定输入，不追认本轮完成了其来源阅读或重建；后续 Mathematical Audit、Writing Audit、发表版本比较、迁移检验及技能更新均未执行，不表示整轮训练完成。

## 任务7

**甲：结论不成立，不能靠表达润色修复。** 序列确实收敛于 \(1\)，但一个递增序列的极限不必是其所在集合的极大元。\(2\in[0,2]\) 且 \(2>1\)，直接否定了所称极大性。建议明确标出最后一步推论错误，不将“集合闭”当作极大性的依据；在不改变原命题的要求下，无法补成成立的证明。

**乙：给定条件足以支持结论，补一行估计即可。** 因 \(T_n\) 连续且非零，\(0<\|T_n\|<\infty\)，故对每个 \(n\)，

\[
|T_nu|
\ge |T_nu_n|-|T_n(u-u_n)|
\ge b_n-\|T_n\|\|u-u_n\|
\ge \frac{b_n}{2}.
\]

若 \(b_n\to\infty\)，则 \(|T_nu|\to\infty\)。这里关键是题中已经给出的、依赖于 \(n\) 的误差界；仅有 \(u_n\to u\) 本身不足以替代这一步。

## 任务8

该归约中的“双射”和“无需核查函数性质”均不成立。\(K=[0,1]^2\) 是二维正方形，不是三维单纯形。

\[
A(\lambda)=(\lambda_2+\lambda_4,\lambda_3+\lambda_4),
\]

是连续仿射满射，但不是单射。例如

\[
A(1/2,0,0,1/2)=A(0,1/2,1/2,0)=(1/2,1/2).
\]

因此这里没有唯一重心坐标，也不能未经证明使用逆坐标映射。

**保留几何像域 \(K\)。** \(K\subset\mathbb R^2\) 与 \([0,1]\) 的非空、紧、凸性质已有给定；\(f(x,y)=x_1y\) 对各变量分别仿射且连续，因而满足题设方向的拟凹、拟凸条件。若调用相应极小极大结果，应将其准确版本、两个变量的方向及这些条件逐项对应。若另走有限维固定点或覆盖证明，则还须构造并核查所用连续自映射或全部覆盖/面条件；不能将正方形直接当三维单纯形来套接口。

**改用系数域 \(\Delta\)。** 定义拉回函数

\[
F(\lambda,y)=f(A\lambda,y)=(\lambda_2+\lambda_4)y.
\]

所需核查包括系数域、参数化及拉回函数三部分。本例 \(\Delta\) 是由 \(\mathbb R^4\) 的四个标准基向量生成的三维标准单纯形，非空、紧且凸；\(A\) 连续仿射且满射。\(F\) 分别连续，对固定 \(y\) 关于 \(\lambda\) 仿射，故拟凹；对固定 \(\lambda\) 关于 \(y\) 仿射，故拟凸。这些性质已在本例直接核对，并非由“换到 \(\Delta\)”自动免检。

回传时取 \(x=A\lambda\)。由于满射且 \(F=f\circ(A,\mathrm{id})\)，同一纤维上的函数值相同，例如对每个 \(y\)，

\[
\sup_{\lambda\in\Delta}F(\lambda,y)=\sup_{x\in K}f(x,y).
\]

其他涉及原域极值或鞍点的输出也须用这一满射关系逐项回传；若使用辅助映射或覆盖，还须核其各自接口。双射并非这种向前回传的必要条件。

本轮只核查给定例子的几何归约、拉回性质与回传责任；没有复原原始论文的证明，也没有重新认证整篇 Sion 定理。

## 任务9

段落 B 更容易核查。它展示了乘积差的分解，并明确指出 Hölder 不等式和 \(v_n\) 的 \(L^2\) 有界性分别承担什么作用。这里有界性确由强收敛得到：

\[
\|v_n\|_2\le\|v_n-v\|_2+\|v\|_2,
\qquad \sup_n\|v_n\|_2<\infty.
\]

因此 B 的估计中两项均趋于零。A 的结论在给定条件下同样成立，但省略了这一可核查的机制。

本轮支持的一条暂时性观察是：当乘积收敛承担当前论证的关键责任时，写出差的分解及“趋零因子 × 有界因子”的估计，能让读者更直接地核对所需输入。其依据仅为本题这一单元，可记为局部观察，不能升级为已验证的可迁移规则；也不意味着所有标准步骤都应展开。若相应估计前文已给出或对目标读者确属惯用结果，A 式简写也可能足够。本例依赖同一域上的双强 \(L^2\) 收敛，不能据此推广到弱弱收敛、不同域或不匹配的指数。

本轮仅完成所给段落的数学依赖核对与表达比较；未选择其他论文、未执行后续迁移、未保存技能或上传。

## 实际读取记录

工作目录为 `WORKSPACE`。下列文件按本轮各题需要集中读取，不表示逐题重复读取；训练契约首次批量输出有局部截断，随后已单独完整读取。

任务材料：

- `validation/behavior-cases.md`

技能主文件：

- `fusion/mathematical-writing/SKILL.md`
- `fusion/mathematical-reasoning/SKILL.md`
- `fusion/math-paper-workflow/SKILL.md`

引用文件：

- `fusion/math-paper-workflow/references/local-preferences.md`
- `fusion/mathematical-writing/references/language-routes.md`
- `fusion/mathematical-writing/references/research-framing.md`
- `fusion/mathematical-writing/references/journal-adaptation.md`
- `fusion/mathematical-writing/references/training-contract.md`
- `fusion/mathematical-reasoning/references/audit-domains.md`
- `fusion/mathematical-reasoning/references/validated-rules.md`
- `fusion/mathematical-reasoning/references/rules/SION-M03.md`
- `fusion/mathematical-reasoning/references/rules/MR-O002.md`
- `fusion/mathematical-reasoning/references/rules/MR-O001.md`
- `fusion/math-paper-workflow/references/proof-grounded-writing.md`

本轮数学推理入口与操作卡所标整合版本为 `2026.10.24-fusion.2`。只采用了其中当前题目适用的检查责任，未核验其历史证据或对技能本身作评价。
