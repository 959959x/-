# 椭圆与非局部正则性写作增补

以下提供公开来源及条件性的证明组织建议，不认证全文数学正确性。数学引用应回到对应原文核对假设；不得把文体范例当成当前方程已满足条件的证据。

## 1. Ovidiu Savin：小扰动与紧性改进

**文献**：Ovidiu Savin, *Small Perturbation Solutions for Elliptic Equations*, Communications in Partial Differential Equations 32(4–6), 557–578 (2007), DOI: 10.1080/03605300500394405。

- [作者公开刊本PDF](https://www.math.columbia.edu/~savin/Small_pert.pdf)
- [作者发表目录](https://www.math.columbia.edu/~savin/papers.html)
- [出版社记录](https://www.tandfonline.com/doi/abs/10.1080/03605300500394405)
- 方法影响依据：Armstrong–Silvestre–Smart 的 *Partial regularity of solutions of fully nonlinear, uniformly elliptic equations*, CPAM 65 (2012), 1169–1184，摘要明确说其论证结合了 Lin 的估计与 Savin 的小扰动正则性结果；参考文献10指向本篇。[后续原始研究](https://onlinelibrary.wiley.com/doi/abs/10.1002/cpa.21394)

**相关位置**：§1，刊页557–560/PDF第1–4页；§2路线图与Lemma 2.1，560–562/第4–6页；§3，568–570/第12–14页；§4与Proposition 4.1证明，571–573/第15–17页；§5.1开头，574–575/第18–19页。

**可推广的写法**：先说明常见方法在哪一步缺少先验控制；引理前交代几何构造及方程真正被使用的位置；把振荡控制、缩放版本、紧性极限和单尺度二次逼近分层；反证末尾不只给出极限方程，而是调整近似多项式使其重新满足原方程的约束，再获得矛盾。

**适用边界**：小扰动、算子的局部一致椭圆性及光滑性是数学前提，不能从这一写作范例推断任意非线性椭圆方程均有相同正则性。

## 2. Luis Caffarelli、Luis Silvestre：非局部正则性与依赖分支

**文献**：Luis Caffarelli and Luis Silvestre, *Regularity Theory for Fully Nonlinear Integro-Differential Equations*, Communications on Pure and Applied Mathematics 62(5), 597–638 (2009), DOI: 10.1002/cpa.20274。

- [作者公开刊本PDF](https://www.math.uchicago.edu/~luis/preprints/Regularity%20theory%20for%20nonlocal.pdf)
- [出版社正式记录](https://onlinelibrary.wiley.com/doi/10.1002/cpa.20274)
- [arXiv记录](https://arxiv.org/abs/0709.4681)
- 方法影响依据：两位作者后续的 *Regularity Results for Nonlocal Equations by Approximation*, ARMA 200 (2011), 59–88，明确以此前平移不变情形的结果配合紧性与扰动方法处理更一般方程，并在参考文献2列出本篇。[后续原始研究](https://link.springer.com/article/10.1007/s00205-010-0336-4)

**相关位置**：§§1–2，刊页597–602/PDF第1–6页；§7，616–617/第20–21页；§8的路线、Lemma 8.1及证明、Lemma 8.4/Corollary 8.5、覆盖构造与Remark 8.8的相关部分，617–623/第21–27页；§9开头的构造目的，623/第27页；§§10–13，625–635/第29–39页。此定位不代替§§3–6、§9或§14中的依赖核查。

**可推广的写法**：长文在进入核心理论前增设依赖路线图；把非局部定义中的域外数据写明；每个障碍后说明新增假设如何解决它；差商局部化时明确列出远场误差和核的控制条件；若强调极限参数的一致性，应在关键引理中持续追踪常数。

**关键依赖核查**：§11明确说明Harnack一节不是后续正则性证明的必经环节；§12直接使用Theorem 10.4，§13再利用Hölder估计处理差商。因此应写成“点到测度估计分别导向Harnack与Hölder；Hölder再导向更高正则性”，不能把所有结果排成一条虚假的串行链。

**适用边界**：全空间数据、核类别、平移不变性与差商所需额外核条件应分清；不得将局部方程中的截断、边界条件或小范围控制直接照搬到非局部情形。

## 3. 按需检查项

1. **改进型证明**：单列单尺度命题，写清归一化、误差大小、缩放后算子、可重复使用的假设，以及如何从一步改进恢复最终正则性。引用范例中的简写不能代替当前项目必要的迭代说明。
2. **紧性反证**：依次给出反例序列、统一控制、收敛拓扑、极限方程、极限的较强性质，以及把近似对象搬回原序列的方法；不要止步于“由紧性得矛盾”。
3. **几何接触论证**：在技术计算前说明接触集合是什么、它如何提供方程信息、测度估计要解决哪个下一步目标。
4. **非局部局部化**：截断或差商前先核查全局定义域；正文须显示新产生的域外积分/误差及其控制，不能只处理球内部分。
5. **真实依赖图**：区别主线、独立分支和可跳读模块；不要把章节先后顺序当成定理间逻辑依赖。
6. **参数一致性**：若结果需要在方程阶数或尺度趋近某极限时仍有效，逐个关键引理注明常数依赖；对不随缩放保持不变的参数单独提醒。

这里只保留独立概括与出处，不复制论文特色句子。两篇提供证明叙述方法，不提供用户项目已经满足某假设或已经证明某结论的证据。
