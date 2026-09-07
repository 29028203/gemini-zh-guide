# Gemini CLI扩展怎么装？MCP、自定义扩展、自定义命令，三层玩法全解

> 原文链接：[https://www.hxsf.com.cn/chajian/2561](https://www.hxsf.com.cn/chajian/2561)

<p>同事装完 Gemini CLI，打了两周字面聊天就把它晾在一边，总结陈词是&#8221;不觉得比网页版强多少&#8221;。我扫了眼他的用法：天天手敲几十字的重复指令，MCP 没配，扩展没装，相当于买了辆手动挡，只在一档起步。论免费额度，Google 对这工具给到个人账号每分钟 60 次、每天 1000 次请求，放在同类里算相当大方。但真正把效率差距拉开的，是它那套一层深过一层的扩展体系。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/08/20260825010504_944408.png" alt="Gemini CLI 扩展系统"></p>
<h2>头一层：MCP 服务器，一句话唤出工具</h2>
<p>MCP（Model Context Protocol）是 CLI 连接外部能力的主通道。配置落在 <code>~/.gemini/settings.json</code>，写好之后在对话里用 <code>@服务器名</code> 就能直接调用。官方 README 给的例子足够直观：敲&#8221;@github 列出我打开的 PR&#8221;、&#8221;@slack 把今天的提交摘要发到开发群&#8221;，CLI 便会去调对应工具干活。</p>
<p>热门玩法里有一条是接媒体生成：借助 vertex-ai-creative-studio 的 mcp-genmedia，终端里直接唤 Imagen 画图，Veo 出视频，Lyria 做音乐，全程不用切去开浏览器。</p>
<h2>第二层：自定义扩展，把命令集打包随身带走</h2>
<p>MCP 解决的是&#8221;用别人的工具&#8221;，自定义扩展（Custom Extensions）对应的就是&#8221;造自己的工具&#8221;。把一组命令，脚本，配置封装成可分享的扩展包，团队其他人一条命令装走。官方备有 Writing Extensions 专门文档讲开发规范，想把团队内部工作流标准化的，用它正合适。</p>
<h2>第三层：自定义命令，成本最低的复用</h2>
<p>若只是想固化几个常用 prompt，扩展系统都不必惊动，Custom Commands 足矣。把复杂指令写成可复用命令，一个斜杠触发，免得每次手敲几十字的需求描述。三层里上手门槛最低的就是它，建议从这儿起步。</p>
<p>三层怎么挑，一句话讲透：接现成能力上 MCP，团队共享靠扩展，个人提效用自定义命令。配置细节可留意站内<a href="https://www.hxsf.com.cn/chajian" target="_blank" rel="noopener">插件</a>栏目的后续拆解，MCP 的 settings.json 写法、扩展的目录结构，之后都会单独开篇。</p>
<p>安装顺带一提：npx @google/gemini-cli 免安装直接跑，npm 全局安装或者 brew install gemini-cli 也都行。stable 渠道逢周二更新。想尝鲜跟 preview 渠道，同样周二发，只是比 stable 晚几个小时。</p>

---

原文链接：[https://www.hxsf.com.cn/chajian/2561](https://www.hxsf.com.cn/chajian/2561)
