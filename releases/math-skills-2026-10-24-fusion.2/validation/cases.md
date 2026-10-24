# 独立任务材料

以下六项互相独立，请分别完成用户请求。使用分配给你的技能目录，不联网，不读取另一版本或评估结论。若请求需要当前外部信息但本轮无法访问，按技能处理。把可交付文字和必要说明存入你的结果文件。记录实际读取的skill/reference路径；不要补造验证或阅读经历。

## 任务1

$mathematical-writing 请仅润色下面这句中文，不翻译、不补证明。原文：设Ω是一个有界区域，假定u_n在L²(Ω)里面强收敛到u，那么u_n⊗u_n在L¹(Ω)中强收敛到u⊗u。

## 任务2

$mathematical-writing 根据以下已给定的数学基线，起草一段中文引言结尾，约180字，不开展新推导。模型记作M。结果A：在Ω为二维有界光滑区域、齐次Dirichlet边界、u₀∈H¹₀(Ω)时，对每个u₀存在唯一全局强解。结果B：若另外满足u₀∈H²(Ω)∩H¹₀(Ω)，离散解在T>0上满足sup_{0≤t≤T}‖u_h(t)−u(t)‖_{L²}≤C(T,Ω,‖u₀‖_{H²})h，C不依赖h；不主张对T一致。资料未提供与前人定理的比较，也未说明证明创新，请不要虚构这些信息。

## 任务3

$mathematical-writing Write one short English paragraph discussing theory and computation. The supplied theorem for the heat equation u_t=u_xx on (0,1), with homogeneous Dirichlet boundaries, states L² contractivity for its solution semigroup. An explicit finite-difference experiment with Δt/Δx²=0.4 showed decreasing error on three grids for one smooth initial profile; one run at 0.6 grew. These runs are the only numerical evidence supplied. The manuscript has not proved a discrete stability theorem. Keep the theoretical result and numerical observations distinct.

## 任务4

$mathematical-writing 请将下面的证明说明缩短为连贯中文，但保留必要条件与缺口，不新增证明：在已经合法建立的近似序列中，对每个n有‖u_n‖_{L∞(0,T;L²)}≤C(T)，这个常数不依赖n，但是可能依赖T。我们还得到了u_n在L²(0,T;L²)中强收敛到u。本文尚未核实u在t=0的时间迹，所以不能据此宣称已经建立全部初始条件。请不要将这一缺口藏到附录。

## 任务5

$mathematical-writing 我准备向Nature Communications首次投稿，请仅起草一段英文cover letter贡献说明和作者需要补充的事实清单。给定材料：本文针对模型M在条件H下证明适定性；研究团队做了两组数值检验。没有提供已有文献对照、所有作者同意声明、利益冲突、数据或代码仓库信息。本轮不能联网；若你无法核当前期刊规定，请说明核对范围，不自行宣布已符合要求。

## 任务6

$mathematical-writing 本次是论文训练的隔离写作阶段。冻结数学骨架：Ω有界，a_n→a且a_n,a≥0；f∈L²(Ω)；结论a_n f→af在L²(Ω)中；机制为范数齐次性‖(a_n−a)f‖₂=|a_n−a|‖f‖₂。请写中文短命题及证明，记录本次到达的阶段，不打开发表版本，不声称已完成后续审查、比较或训练。
# 补充任务材料

各项独立完成，只用分配的技能目录与下面的材料，不联网，不读取其他技能版本、评估意见或测试结果。不向外写入，也不修改技能。分别给出用户可用的回答，并简短记录实际读取的文件。

## 任务7

$mathematical-writing 请审查下面两段证明的表达是否足以支持结论，并给出简短修改建议；不改变数学命题，不把缺失证明默认为已知。

甲：在通常大小关系下考虑集合 [0,2]，取 x_n=1−1/n。序列递增且为 Cauchy，集合闭，所以 x_n→1，故 1 是 [0,2] 的极大元。

乙：X 是 Banach 空间，T_n∈X* 非零且连续。已构造 u_n→u，每个 n 有 |T_n u_n|≥b_n>0，且 ||u−u_n||≤b_n/(2||T_n||)。因此 |T_n u|≥b_n/2；若 b_n→∞，则这些峰值发散。

## 任务8

$mathematical-reasoning 请审查这条有限凸几何归约是否成立。令 a_1=(0,0)、a_2=(1,0)、a_3=(0,1)、a_4=(1,1)，K=conv{a_1,a_2,a_3,a_4}，Δ={λ∈R⁴:λ_i≥0, Σλ_i=1}，A(λ)=Σλ_i a_i。作者写：“K 由四个点生成，所以 K 本身就是三维单纯形，每一点有唯一重心坐标；因此把 K 上的问题改写到 Δ 既是双射，也不需要再核查函数性质。”

随后考虑 K×[0,1] 上的 f(x,y)=x_1 y。已给事实：两个域非空、紧且凸；f 实值并分别连续，对固定 y 关于 x 拟凹，对固定 x 关于 y 拟凸。请说明可以保留原像域 K 的做法与使用 Δ 的做法分别需要什么核查，不引用原始论文未提供的证明细节，不宣称重新认证整篇 Sion 定理。

## 任务9

$math-paper-workflow 本次只做限定学习：比较以下两个段落哪一个更容易核查，并从这个小例子给出一条暂时性的写作观察。不要继续选论文、保存技能或上传。

已知 u_n→u 于 L²(Q)，v_n→v 于 L²(Q)。段落A：“由收敛性，u_nv_n→uv 于 L¹(Q)。”段落B：“将差拆为 (u_n−u)v_n+u(v_n−v)，利用 Hölder 不等式和 v_n 的 L² 有界性，得到 ||u_nv_n−uv||₁≤||u_n−u||₂||v_n||₂+||u||₂||v_n−v||₂→0。”

请给出本轮能支持的观察和适用边界；本轮没有其它论文材料，也没有后续迁移任务。
