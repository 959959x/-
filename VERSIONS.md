# 原版与融合版

仓库并存两套数学论文技能。原版保留在原位置，融合版独立放在`fusion/`。

| 版本 | 技能目录 | 说明与完整性清单 |
|---|---|---|
| 原版：2026.10.10 | [skills/](skills/) | [中文说明](README.zh-CN.md)、[MANIFEST](MANIFEST.json)、[SHA256SUMS](SHA256SUMS) |
| 融合版：2026.10.10-fusion.1 | [fusion/skills/](fusion/skills/) | [中文说明](fusion/README.zh-CN.md)、[MANIFEST](fusion/MANIFEST.json)、[SHA256SUMS](fusion/SHA256SUMS) |

融合版保留原有数学推理、证明组织与训练契约，新增数学摘要、引言、贡献定位、意义与边界、理论与数值主张区分及按需期刊/首次投稿适配。来源和迁移范围见[融合记录](fusion/skills/mathematical-writing/references/fusion-provenance.md)。新增建议没有自动升为Level2/3，有限行为试验不认证整篇数学证明。

## 下载与安装

下载整个仓库ZIP并解压：

- 使用原版：复制仓库根目录`skills`内的三个技能文件夹。
- 使用融合版：先进入`fusion`，再复制该目录`skills`内的三个技能文件夹。

三个文件夹为`math-paper-workflow`、`mathematical-reasoning`、`mathematical-writing`。按对应版本中文说明安装到本机技能位置。两版名称相同，只选一套，避免复制时相互覆盖；并存于GitHub不代表应在本机重复安装。

## 完整性与版本保留

根目录的MANIFEST和SHA256SUMS继续用于原版载荷；融合版清单以`fusion/`为包根目录，核验时先进入该目录。根目录原有文件未为本次发布重写，其Git blob与原版提交`40ea90ddf14eda1202fde85745d51cef2993b0c6`一致。

本次仅新增`fusion/`和本版本说明。此前替换根目录技能的草稿PR #2由此次并存发布取代。原版还可通过[固定历史版本](https://github.com/959959x/-/tree/40ea90ddf14eda1202fde85745d51cef2993b0c6)访问。
