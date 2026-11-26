# Scientific PPT

`scientific-ppt` 是一个用于科研口头汇报的 Codex 技能。它可以制作、改写或审阅组会、文献汇报、答辩和学术报告的幻灯片。

## 汇报设计

- 按研究问题、关键证据和阶段结论推进故事，把转场和详细解释写进讲者备注。
- 默认采用白底、蓝色结论标题和横线、黑色正文。把主要结论放在标题位置，用一张主图或一组直接比较支撑，省去固定的页底总结。
- 裁选论文图中与本页结论相关的部分，保留必要的对照、单位和实验条件。
- 默认静态呈现。动画能说明时间变化、空间对应或机制时，先写动画脚本，再用 PowerPoint 原生动画制作，逐步放映检查并随演示交付脚本。制作原生动画需要可操作的 PowerPoint 环境。

## 安装与使用

在 macOS 或 Linux 的终端中，将仓库克隆到 Codex 的个人技能目录。

```bash
mkdir -p "$HOME/.agents/skills"
git clone https://github.com/flyingsand/scientific-ppt.git "$HOME/.agents/skills/scientific-ppt"
```

在 Codex 中用 `$scientific-ppt` 调用技能。提供听众、时长以及论文或现有 PPT，有助于安排讲解节奏。例如可以发送下面这条请求。

> $scientific-ppt 请根据这篇论文制作一份 12 分钟的组会 PPT。听众熟悉这个领域。用论文中的关键图解释研究问题、方法和证据，并在讲者备注中写好转场。

安装位置见 [Codex 官方技能文档](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)。

## 技能文件与来源

- [SKILL.md](SKILL.md) 收录版式、内容取舍、叙事和交付规范。
- [论文图改稿示例](references/examples.md)、[统计图样式](references/chart-style.md)和[动画流程](references/animation-workflow.md)提供具体参考。
- 本技能独立整理自 Susan McConnell 的公开课程。讲义例图及其图内素材的权利归原作者或权利人。讲义和课程链接见[来源说明](references/sources.md)。
- 三张统计图样式例图裁自 Qiushi Han、Keya Hu、Linlu Qiu、Cathy Wu 和 Kaiming He 的 VISTA 论文图 5、6(b) 和 9(b)。[论文](https://arxiv.org/abs/2610.02200v1) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
