# Gemini CLI 发版节奏：stable 每周二转正、preview 先行、nightly 尝鲜

> 原文链接：[https://www.hxsf.com.cn/geminidt/2611](https://www.hxsf.com.cn/geminidt/2611)

<p><a href="https://www.hxsf.com.cn/geminidt" target="_blank" rel="noopener">Gemini CLI</a> 进入了密集发版期。仓库信息显示，最新文档已经更新到 v0.59.0-preview.0，v0.60.0-nightly 版本也在 9 月初发布。对正在用或者准备用 Gemini CLI 的人，把它的版本节奏搞清楚，选渠道就不纠结了。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190700_086645.png" alt="Gemini CLI版本节奏"></p>
<p>三个发布渠道分工明确。stable 稳定版每周二正式推送，相当于把上一周的 preview 转正，同时修掉验证阶段发现的问题。preview 预览版每周二先行发布，新功能先在这里出现。nightly 每日更新，直接同步主分支当天的所有改动，未经充分验证。</p>
<p>选哪个渠道看用途。日常干活用 stable 最稳。想提前体验新功能，用 preview。自己也是贡献者，或者愿意踩坑反馈的，才考虑 nightly。安装方式上，npm 全局安装 @google/gemini-cli 就行，也可以用 npx 直接跑，Homebrew 和 conda 也支持。</p>
<p>从仓库提交记录看，近期更新集中在几个方向。MCP 集成做了加固，受限模式下工作区信任改为默认不信任，并对 MCP 服务器做过滤，降低恶意配置的风险。Chrome DevTools MCP 组件清理了硬编码的 CrUX API 密钥，安全上更干净。日常的 bug 修复和依赖更新在持续滚动。</p>
<p>官方维护了完整的 Changelog，每次 preview 发布都会同步更新说明。想跟版本的，订阅仓库的 release 通知，或者每周二看一眼 Changelog 就够了。</p>
<p>还不熟悉 Gemini CLI 的话，简单补一句它的定位。开源项目，Apache 2.0 协议，把 Gemini 装进终端用。免费档每天 1000 次请求，支持 1M 上下文，可以接 MCP 服务器扩展能力，比如连上 Imagen、Veo 生成图片和视频。它和 Gemini 应用互补，一个在终端里干活，一个在日常对话里干活。</p>

---

原文链接：[https://www.hxsf.com.cn/geminidt/2611](https://www.hxsf.com.cn/geminidt/2611)
