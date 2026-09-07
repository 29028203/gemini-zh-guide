# Gemini CLI 接 MCP 的安全基线：受限模式、信任目录、最小权限

> 原文链接：[https://www.hxsf.com.cn/jiaocheng/2615](https://www.hxsf.com.cn/jiaocheng/2615)

<p>给 <a href="https://www.hxsf.com.cn/geminidt" target="_blank" rel="noopener">Gemini CLI</a> 接上 MCP，等于给一段没见过的代码，开了个能指挥 AI 动工具的权限。这段代码靠得住，干活确实方便。靠不住，麻烦就大了。Gemini CLI 最近几个版本的安全更新，值得花十分钟弄明白。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190717_915501.png" alt="Gemini CLI安全配置"></p>
<p>先看权限。现在默认谁都不信，只有你自己加进白名单的目录才会放行。挂在配置里的 MCP 服务器同样要过一遍筛子，不是谁都能进。</p>
<p>再看目录。项目文件夹放进信任区，AI 才能在里面执行命令。下载文件夹、系统文件夹别放进去。提示词里就算混进坏东西，AI 也出不了信任区那圈范围。</p>
<p>还有 MCP 本身。配置里挂一堆用不上的服务器，等于多开几扇门。只挂正在用的，用完删掉。来源也挑一挑，官方和口碑好的优先，网络权限、文件权限能缩多小缩多小。Chrome DevTools 那个组件最近把写死的密钥清了，这种自查越多越好。</p>
<p>几条容易踩的坑顺带说下。网上流传的 GEMINI.md、MCP 配置模板，喂给 AI 之前先自己扫一眼。密码类的变量别写进项目配置。要跑陌生的代码，先扔进容器里。</p>
<p>这套东西配好花不了十分钟。配好之后，工具照常用，心里也踏实。</p>

---

原文链接：[https://www.hxsf.com.cn/jiaocheng/2615](https://www.hxsf.com.cn/jiaocheng/2615)
