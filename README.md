# Claude Code 视频 Skills 使用手册

**在线看：<https://cyberhandyman.github.io/video-skills-handbook/>**

7 个“用 Claude Code 写代码做视频”的 skill 的使用手册：每个 skill 怎么用、有哪些风格、在 Claude Code 里怎么写 prompt。手册里一共收了 384 种风格 / 画法 / 镜头卡，每张卡都能点开看样片，一键复制 prompt，改掉【】里的内容就能粘进 Claude Code 用。

这些 skill 的思路都一样：Claude 写网页 / Canvas / WebGL / Remotion 代码画出每一帧，用无头浏览器逐帧截图，再用 ffmpeg 合成 mp4，配乐多半也用代码合成。不用生图或视频生成模型。

| # | Skill | 适合做什么 | 作者 | 许可 |
|---|---|---|---|---|
| 1 | [xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | 最通用：给想法、文章或参考片，先出 3 套方案和预览，选定后做成片 | 周行 · Kianzzz | MIT |
| 2 | [lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | 影片风格图册：51 种库风格 + OPUSCAR 98，报出风格名就照着拍 | LemoLab | MIT |
| 3 | [mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) | 15 种 MG 动态设计风格，每种一支 10 秒原片、完整提示词和源码 | Vincentwei1021 | MIT |
| 4 | [dashi-animationstyle](https://github.com/chuspeeism/dashi-animationstyle) | 给 15–60 秒中文口播配动画画面，带字幕，能直接拖进剪映 | Dashi AI Lab | MIT |
| 5 | [huashu-art-motion](https://github.com/alchaincyf/huashu-art-motion) | 美术史画风动画（36 种实做风格 + 17 张研究配方）+ 9 种解说动画语法 | 花叔 · alchaincyf | MIT（花叔形象、Clawd 除外） |
| 6 | [wtt-code-animation-studio](https://github.com/WaterDJiang/Wattter_openSkills/tree/main/wattter_skills/wtt-code-animation-studio) | 从编剧开始：剧本、分镜、可改源码、带配音的成片一次交齐 | Water · WaterDJiang | CC BY-NC-SA 4.0 |
| 7 | [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | 把网页 / 前端项目拍成 2.5D 运镜产品宣传片，124 张镜头配方卡 | Vincentwei1021 | Apache-2.0 |

## 手册里有什么

- **选型速查**：我要做什么 → 用哪个 skill；外加一张横向对比表。
- **通用 prompt 写法**：一条好 prompt 的组成、三种叫出 skill 的方式、出片后怎么改。
- **风格总库**：7 个 skill 的全部风格放在一起，可以筛选、搜索；网格里是静音预览，点开看原片和完整 prompt。
- **逐个 skill 详解**：适合 / 不适合、规格与环境、工作流程、Prompt 模板、风格卡、样片、技巧与坑。

## 样片与版权

- 网页里能直接播放的样片来自各作者的仓库、Releases 或展示站，按原仓库许可转载，许可文本放在 [`licenses/`](licenses/)。视频都压成了 720p 网页版，原画质请到作者仓库看。
- 这些内容不在开源许可范围内，**只放缩略图，点开跳到原地址**：
  - 作者发在 X / YouTube 上的作品；
  - README 致谢的他人案例；
  - video-shotcraft showcase 里的社区投稿；
  - huashu-art-motion 声明不随 MIT 授权的花叔形象和 Clawd 同人片。
- wtt-code-animation-studio 的作者没有发布样片，这里的是用该 skill 自己的流水线渲染的示意片，画面上标了“示意”。
- huashu-art-motion 的一部分风格样片，是用作者公开的场景代码渲染的；每张卡的“样片来源说明”写清了哪些是作者原片。
- 所有样片的版权归各原作者。如果有不妥，请开 issue，会尽快处理。

## 目录

- `index.html`：手册网页（数据内嵌；克隆仓库后离线也能打开）
- `样片库/`：网页版样片，按 skill 编号分文件夹
- `licenses/`：各仓库的许可文本

本仓库由本地脚本从同一份数据生成，内容和本地版手册一致。
