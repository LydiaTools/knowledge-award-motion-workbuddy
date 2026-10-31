# Knowledge Award Motion for WorkBuddy

[中文介绍](#中文介绍) · [Download the Skill package](knowledge-award-motion-分享候选.zip)

Create editable, black-and-gold probability explainer videos with WorkBuddy or Codex. This adaptation provides a reusable HyperFrames project and scripts for independent repeated-trial problems.

## What it does

- Generate animated question cards, trial grids, failure chains and probability curves in 1920 × 1080.
- Change the per-trial probability and trial count; the project computes the result using **1 − (1 − p)ⁿ**.
- Produce a video with instrumental music and retain the editable source project.

## Get started

1. Download and unzip the [complete Skill package](knowledge-award-motion-分享候选.zip). Copy the entire `knowledge-award-motion` folder into your assistant's skills directory and refresh its skill list; keep its files together.
2. Install Node.js 22, Chrome/Chromium, FFmpeg and FFprobe. In the skill folder run `npm install` to install HyperFrames and its dependencies.
3. Ask your agent to read the Skill and create an independent-probability project, or run the commands in `SKILL.md`. Inspect the assumptions, generated video and music before publishing.

The current tested template supports independent repeated trials with a constant probability. Different knowledge topics may require new scene code and review; it does not automatically turn every topic into a completed video. A local parameter-change render was tested using the existing HyperFrames installation; a fresh-machine installation has not yet been verified.

## Credits and licensing

Adapted from the local WorkBuddy version of Lemo-Opuscar and its knowledge-video workflow. The upstream MIT license and authorship are retained in the package. Fonts, Three.js, GSAP and other third-party dependencies keep their respective notices and terms; see `CREDITS.md` inside the package. Reference creators' videos and audio are not included.

## 中文介绍

这是一个面向 WorkBuddy 和 Codex 的黑底知识动画 Skill 适配包。已实现的概率视频模板可设置单次成功概率和尝试次数，自动生成标题、点阵、失败概率和累计概率曲线，并导出带配乐的横屏视频及可编辑工程。

**安装方式：**下载 [完整 Skill 压缩包](knowledge-award-motion-分享候选.zip)，解压后将整个文件夹放入助手的 Skill 目录，保留其中的脚本和资源。安装 Node.js 22、Chrome/Chromium、FFmpeg 和 FFprobe，在 Skill 目录执行 `npm install`；具体命令见包内 `SKILL.md`。

**使用边界：**计算适用于每次相互独立且成功概率不变的情况；点阵是程序生成的可视化，不是真实用户数据。其他知识题目需要根据事实与分镜制作或修改场景，不能仅改标题。本机已完成更换参数后的实际渲染；暂未验证全新电脑从零安装。配音与其他素材请使用有权使用的资源。

**来源与许可：**基于本机 Lemo-Opuscar WorkBuddy 适配版及知识视频工作流整理；包内保留上游许可与署名，字体、动画库及其他第三方资源遵循各自许可。参考作品的视频与音频未收录。
