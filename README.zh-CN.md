# 数学论文技能：本地可移植版

用于中英文数学/PDE论文润色、证明审查与结构组织。下载后复制三个文件夹即可使用，不需要 Python 或安装脚本。

## Windows 安装

1. 在 GitHub 仓库页点 **Code → Download ZIP**，解压。
2. 打开解压后的 `skills` 文件夹，将里面这三个文件夹一起复制：
   - `math-paper-workflow`
   - `mathematical-reasoning`
   - `mathematical-writing`
3. 放到运行 Codex 的当前用户目录 `$HOME/.agents/skills/`。原生 Windows 通常是：
   `C:\Users\<用户名>\.agents\skills\`
   最终应能找到：`C:\Users\<用户名>\.agents\skills\mathematical-writing\SKILL.md`。
4. 重新查看技能列表；若未出现，重启 Codex。在 Codex CLI/IDE 中用 `/skills` 查看，或输入 `$mathematical-writing` 调用。

只想让某个项目使用时，可改放 `项目目录/.agents/skills/`。两种位置选一种，避免同名重复。不要把外层 `skills` 文件夹再套一层后复制。

如果 Codex 在 WSL 中运行，用 WSL 自己的 `$HOME/.agents/skills/`，而非默认 Windows 用户目录。旧版本或旧安装器可能仍使用 `~/.codex/skills`；以本机实际发现结果为准，不要同时安装两份。

安装位置与调用方式按 [OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills) 核对（2026-10-10）。这是本地目录式安装包。

## 先做一个小测试

向 Codex 发送：

> $mathematical-writing 请仅润色下面这句英文，不翻译、不补证明、不训练，也不修改技能文件；保留假设、量词与结论强度。原文：Let Ω be a bounded domain. Assume that u_n converges strongly to u in L²(Ω). Then u_n⊗u_n converges to u⊗u in L¹(Ω).

检查它是否只返回更清楚的英文及必要说明，保留“有界域、强 L² 收敛、L¹ 张量积收敛”，没有自动启动论文训练。此测试检查安装和任务分流，不认证数学能力或所有规则的效果。

## 三个入口怎么选

- `$mathematical-writing`：中英文润色、定理/证明组织、章节衔接和结构审查
- `$mathematical-reasoning`：推导与证明审查，检查假设、空间、估计、算子域、极限和闭合
- `$math-paper-workflow`：综合入口，让任务按需要分流

普通润色和翻译只处理给定内容；数学疑点单列，不暗中更改结论。只有明确要求论文训练时才启用训练契约。训练、持续选文、修改技能和外部上传不会因安装而自动开始。

三个技能有相互引用，请一起复制。每个技能的 `SKILL.md` 是入口；`references` 是按需加载的规则和范例，不必每次全部阅读。`agents` 与 `assets` 是显示信息和图标。纯文本任务无需额外软件；若要求编译 LaTeX、生成 PDF 或联网核文献，需本机相应工具与访问能力。

## 导出内容与边界

发行号：2026.10.10。

本包提供三个技能的使用规则、必要参考文件与公开文献定位，不包含训练过程记录、第三方论文全文或账号信息。按需使用数学推理、论文组织与语言润色功能。

Level 3 / validated 是范围受限支持，非 strong、非自动定理、非普遍最优；Level 2 候选不能当成强制模板。来源摘要不代表当前使用者已读原文。新任务必须重新核对实际数学条件。

## 文件完整性

`MANIFEST.json` 仅列包名称、发行号及载荷文件的相对路径、字节数和 SHA-256；为避免自递归，不列自身与 `SHA256SUMS`。`SHA256SUMS` 覆盖载荷与 `MANIFEST.json`，自身不自校验。

需要核验时，在解压目录打开 PowerShell，可对单个文件运行：

```powershell
Get-FileHash -Algorithm SHA256 .\skills\mathematical-writing\SKILL.md
```

将结果与 `MANIFEST.json` 的相同路径记录比较。无需执行下载来的脚本。哈希验证下载后文件是否一致，不证明数学正确性。
