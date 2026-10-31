---
name: knowledge-award-motion
description: 制作黑底横屏知识动画；可复用内置的独立试验概率可视化项目，或以其工程作为知识动画制作参考。用于 WorkBuddy、Codex 等可操作本地文件和运行命令的助手。
---

# 知识动画制作

先检查当前主题、用户要求和来源。确定内容事实、对象动作、画幅、音乐及输出路径；不虚构数据或把生成的点阵称为真实用户统计。检查画面中标题、数值、边界和音频。创建新目录，不覆盖现有工程。

## 已实现的概率项目

针对各次独立、单次概率固定的问题，使用脚本生成原生 HyperFrames 工程。参数为单次成功概率 `--probability`、尝试次数 `--trials`、点组数量 `--groups` 与随机种子 `--seed`。计算按 `1-(1-p)^n`；题目必须真实满足假设。

需要 Node.js 22、HyperFrames 0.8.183、Chrome/Chromium 与可在 PATH 找到的 FFmpeg/FFprobe。首次在本包目录运行 `npm install` 安装依赖；审查依赖来源后再执行。示例：

```bash
node scripts/create-project.mjs --probability 0.01 --trials 100 --groups 1000 --seed 20261031 --out /absolute/path/to/new-project
node scripts/render.mjs --project /absolute/path/to/new-project --out /absolute/path/to/new-film.mp4
```

脚本会把可编辑源工程复制到全新目录，按同一模型计算标题、点阵、失败链、曲线和结论。渲染产生 1920×1080、30fps 的带配乐 MP4。生成的是数学可视化，点阵是程序生成的数据，不是用户调查。配乐可替换为用户有权使用的音频；如需旁白，先使用用户指定并确认的文案与音色。

## 其他选题

本包没有承诺任意选题一键生成。先拆解事实、主体、触发、动作、结果和镜头承接；查阅 `assets/template` 内的场景模块，判断现有组件能否正确表达。无法表达时，应由助手制作新的原创分镜与动画实现，并另行渲染与核查，不能只替换标题或把其他主题伪装为概率题。

## 交付检查

打开最终 MP4 检查主题是否从首帧可见，文字是否遮挡、数值与条件是否一致，声音是否存在、动作是否连续；还应保存生成参数、源工程与成片哈希。程序检查不等于人工完整观看、听审或用户认可。版权和许可见 `CREDITS.md` 及各素材随附的许可。
