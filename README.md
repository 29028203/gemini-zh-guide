# Gemini 中文指南

## Gemini CLI介绍

Gemini CLI 是 Google 推出的开源命令行 AI 编程助手，在本地终端运行，将 Gemini 模型的强大能力直接带入命令行。支持通过自然语言指令查询和编辑大型代码库、从 PDF 或草图生成新应用、自动化操作任务（如查询 PR 或处理复杂 rebase）。Gemini CLI 接入 Gemini 2.5 Pro 模型，具备 100 万 token 超长上下文窗口，专为真实软件工程任务优化，支持多模态输入，可处理文本、图片、PDF 和草图。内置 Google 搜索工具，支持 MCP 协议扩展，可连接 Imagen、Veo 等媒体生成能力。采用 Apache 2.0 开源许可证，支持 Windows、macOS 和 Linux 三大平台，个人 Google 账号登录即享每分钟 60 次、每天 1000 次免费请求。

## Gemini CLI特点

- 终端原生运行，轻量高效，零配置开箱即用。
- Gemini 2.5 Pro 模型驱动，百万 token 超长上下文。
- 支持代码理解、生成、调试、重构全流程开发。
- 多模态输入，支持文本、图片、PDF、草图理解。
- 支持 MCP 协议扩展，内置 Google 搜索与 Shell 工具。

## Gemini CLI教程与指南

- [Gemini CLI 接 MCP 的安全基线：受限模式、信任目录、最小权限](https://www.hxsf.com.cn/jiaocheng/2615) · [📄 仓库内阅读](docs/2615-GeminiCLI接MCP的安全基线：受限模式、信任目录、最小权限.md)
- [Gemini 3.5 Transcribe 怎么用：Mac 应用、安卓 Gboard、Chrome 三条路](https://www.hxsf.com.cn/jiaocheng/2614) · [📄 仓库内阅读](docs/2614-Gemini3.5Transcribe怎么用：Mac应用、安卓Gboard、Ch.md)
- [Gemini 3.8 Flash 现在能不能用：开发者、个人与企业各走哪条路](https://www.hxsf.com.cn/jiaocheng/2612) · [📄 仓库内阅读](docs/2612-Gemini3.8Flash现在能不能用：开发者、个人与企业各走哪条路.md)
- [让Gemini帮你审代码：GitHub官方Action五步配好，@gemini-cli一句话触发](https://www.hxsf.com.cn/chajian/2562) · [📄 仓库内阅读](docs/2562-让Gemini帮你审代码：GitHub官方Action五步配好，@gemini-.md)
- [Gemini CLI扩展怎么装？MCP、自定义扩展、自定义命令，三层玩法全解](https://www.hxsf.com.cn/chajian/2561) · [📄 仓库内阅读](docs/2561-GeminiCLI扩展怎么装？MCP、自定义扩展、自定义命令，三层玩法全解.md)
- [Gemini API省钱攻略：批量模式最高打一折，上下文缓存再砍一刀](https://www.hxsf.com.cn/jiaocheng/2560) · [📄 仓库内阅读](docs/2560-GeminiAPI省钱攻略：批量模式最高打一折，上下文缓存再砍一刀.md)
- [Gemini API官方Cookbook怎么学？49个免费教程和正确的入门顺序](https://www.hxsf.com.cn/jiaocheng/2559) · [📄 仓库内阅读](docs/2559-GeminiAPI官方Cookbook怎么学？49个免费教程和正确的入门顺序.md)

## Gemini CLI版本动态

- 2026-09-07 · [Gemini 3.5 Transcribe发布：85种语言实时转写，词错误率最低2.6%](https://www.hxsf.com.cn/geminidt/2605) · [📄 仓库内阅读](changelog/2605-Gemini3.5Transcribe发布：85种语言实时转写，词错误率最低2..md)
- 2026-09-06 · [Gemini视频理解上新：像分析师一样挑着看视频，token最高省88%](https://www.hxsf.com.cn/geminidt/2604) · [📄 仓库内阅读](changelog/2604-Gemini视频理解上新：像分析师一样挑着看视频，token最高省88%.md)
- 2026-09-05 · [Gemini 3.5 Transcribe 发布：语音转写词错率降到2.6%，输出还自带整理](https://www.hxsf.com.cn/geminidt/2613) · [📄 仓库内阅读](changelog/2613-Gemini3.5Transcribe发布：语音转写词错率降到2.6%，输出还自.md)
- 2026-09-05 · [Gemini CLI 发版节奏：stable 每周二转正、preview 先行、nightly 尝鲜](https://www.hxsf.com.cn/geminidt/2611) · [📄 仓库内阅读](changelog/2611-GeminiCLI发版节奏：stable每周二转正、preview先行、nigh.md)
- 2026-09-05 · [Gemini 视频理解升级：token 消耗最高降88%，长视频分析成本大降](https://www.hxsf.com.cn/geminidt/2610) · [📄 仓库内阅读](changelog/2610-Gemini视频理解升级：token消耗最高降88%，长视频分析成本大降.md)
- 2026-08-26 · [Waymo无人车里装了个Gemini：能调空调，也能讲纪念碑的历史](https://www.hxsf.com.cn/geminidt/2557) · [📄 仓库内阅读](changelog/2557-Waymo无人车里装了个Gemini：能调空调，也能讲纪念碑的历史.md)
- 2026-08-26 · [Waymo无人车装了个Gemini：能调空调能讲历史，但就是不许碰方向盘](https://www.hxsf.com.cn/geminidt/2563) · [📄 仓库内阅读](changelog/2563-Waymo无人车装了个Gemini：能调空调能讲历史，但就是不许碰方向盘.md)
- 2026-08-25 · [Google给学生发福利：Gemini订阅免费一年，Pro套餐也能白嫖](https://www.hxsf.com.cn/geminidt/2556) · [📄 仓库内阅读](changelog/2556-Google给学生发福利：Gemini订阅免费一年，Pro套餐也能白嫖.md)

---

**官方持续更新入口：[Gemini中文站 官网](https://www.hxsf.com.cn/)**

© [Gemini中文站](https://www.hxsf.com.cn/) · 本仓库为官网内容镜像，文章版权归原作者所有。