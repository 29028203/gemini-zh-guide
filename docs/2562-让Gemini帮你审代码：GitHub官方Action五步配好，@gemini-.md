# 让Gemini帮你审代码：GitHub官方Action五步配好，@gemini-cli一句话触发

> 原文链接：[https://www.hxsf.com.cn/chajian/2562](https://www.hxsf.com.cn/chajian/2562)

<p>三个人的小团队，七个待审 PR，最老的一条已经挂了一整周，这是我上周在朋友仓库里看到的景象。指望专门腾个人出来审代码，不现实。解法是我替他把仓库接上 Google 的 run-gemini-cli GitHub Action：新 PR 一开自动过审，issue 进来自动分类打标，评论区 @gemini-cli 还能随口派活。整套接入五步收工，workflow 代码一行没碰，前后只花了十分钟。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/08/20260825010524_954784.png" alt="Gemini 代码审查工作流"></p>
<h2>五步流程，逐步照抄即可</h2>
<p>第一步，去 Google AI Studio 申请 API Key，免费额度应付日常审查绰绰有余。第二步，Key 存进仓库的 GitHub Secrets，路径 Settings → Secrets and variables → Actions → New repository secret，命名 GEMINI_API_KEY。第三步，.gitignore 里追加 <code>.gemini/</code> 与 <code>gha-creds-*.json</code> 两项。第四步最关键也最省力：终端启动 gemini CLI，敲 <code>/setup-github</code>，预构建的工作流便自动部署进仓库。命令行不顺手的，也可以从官方仓库 examples/workflows 目录把 yaml 复制到 .github/workflows，效果一致。第五步，随手开个 PR 验证，几分钟后评论区就会冒出 GEMINI 的审查意见。</p>
<h2>能派出去的活都有哪些</h2>
<p>官方预置四个工作流，各管一摊：PR 一开即触发审查。issue 一到自动分类打标。一个中央调度器负责把事件分发给对应工作流。再配一个通用助手，凡是自然语言描述的任务照单全收。</p>
<p>@gemini-cli 的唤法分两类。斜杠命令绑定固定动作：<code>@gemini-cli /review</code> 拉起 PR 审查，<code>@gemini-cli /triage</code> 给 issue 分类。自然语言则是开放式委派，官方文档给的示例包括&#8221;解释这个代码变更&#8221;&#8221;帮这个函数写单元测试&#8221;&#8221;修复这个 issue&#8221;，最后这种要留神，它是真的会动手改代码并提交的。</p>
<h2>企业接入也没缺位</h2>
<p>企业向的配置给得很足：GCP 服务账户，Workload Identity Federation，Vertex AI 全在支持之列，接自有 Google Cloud 体系没有障碍。版本可以钉死，gemini_cli_version 填具体版本号就行。模型任你指定。也支持先给 CLI 装上<a href="https://www.hxsf.com.cn/chajian" target="_blank" rel="noopener">插件</a>扩充能力，再挂进工作流。官方另有一条白纸黑字的生产建议：Action 版本固定，分支保护启用，PR 审批人限制。说到底，这是放 AI 进仓库提交代码，权限该收紧的地方别手软。</p>
<p>末了两个坑提醒。其一，DEBUG 环境变量千万别设，官方文档警告，这会让 CLI 挂起苦等调试器。其二，仓库根目录备一份 GEMINI.md，把项目规范写进去，审查意见才会贴着你的代码风格说话，而不是输出一堆正确却没用的套话。</p>

---

原文链接：[https://www.hxsf.com.cn/chajian/2562](https://www.hxsf.com.cn/chajian/2562)
