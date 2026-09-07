# Gemini 3.5 Transcribe 发布：语音转写词错率降到2.6%，输出还自带整理

> 原文链接：[https://www.hxsf.com.cn/geminidt/2613](https://www.hxsf.com.cn/geminidt/2613)

<p><a href="https://www.hxsf.com.cn/geminidt" target="_blank" rel="noopener">Gemini 3.5 Transcribe</a> 是谷歌在 8 月 26 日发布的语音转写模型。它跟以前的语音识别不一样的地方，是把转出来的字再整理过一遍，去掉口头语，补上标点，让结果可以直接用。做语音应用、字幕、会议记录的人，可以直接换上来试。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190610_499267.png" alt="Gemini 3.5 Transcribe"></p>
<p>效果上可以拿数字看。第三方测的流式词错率在 4% 上下，非流式更低，只有 2.6%。相比上一代 Chirp 3，最终转写时间提升了约 70%。</p>
<p>语言支持超过 85 种，能自动识别地区口音和方言。预录音频可以区分最多 3 位说话人，并给出时间戳。对中文用户来说，带口音的普通话、夹杂英文术语的会议，还有嘈杂环境里的录音，这些以前容易翻车的场景都是它的优化重点。官方说它在真实世界的嘈杂环境中表现稳定，还能准确抓取邮政编码、订单号这类字母数字实体。</p>
<p>它聪明的地方在会整理。传统语音识别只是把声音变成字，Gemini 3.5 Transcribe 多做了两步。智能转写会自动处理说话人的自我纠正，比如&#8221;周二见面，不对，周三&#8221;，去掉&#8221;嗯&#8221;&#8221;啊&#8221;这类填充词，并自动格式化文本。自定义词汇表能识别专业术语和独特拼写，专业领域的词表可以直接喂给它。它还支持函数调用，转写过程中可以把图像生成、文件分析这类子任务委托给其他 Gemini 模型。</p>
<p>开发者有两条 API 可用。Live API 做实时双向流式转写，亚秒级延迟，适合语音助手和实时字幕。Interactions API 处理录音、会议和通话记录，带说话人归属和时间戳。模型标识分别是 gemini-3.5-transcribe-live 和 gemini-3.5-transcribe，从发布当天起在 Google AI Studio 公开预览。</p>
<p>大众端也已经铺开。Gemini 的 macOS 应用支持语音转写和结合屏幕上下文的语音操作，安卓的 Gboard 新增了 Rambler 功能，说话直接变成格式良好的文字，还能用语音编辑、纠正拼写。Chrome 里边说话边打字的能力也快了。</p>

---

原文链接：[https://www.hxsf.com.cn/geminidt/2613](https://www.hxsf.com.cn/geminidt/2613)
