# Gemini 3.5 Transcribe发布：85种语言实时转写，词错误率最低2.6%

> 原文链接：[https://www.hxsf.com.cn/geminidt/2605](https://www.hxsf.com.cn/geminidt/2605)

<p>8月26日，谷歌发布<a href="https://www.hxsf.com.cn/" target="_blank" rel="noopener">Gemini</a> 3.5 Transcribe，官方直接把它称为&#8221;迄今最精确的语音转文本模型&#8221;。对做语音应用、字幕、会议记录的人来说，这是一次实打实的能力换代。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190610_499267.png" alt="Gemini 3.5 Transcribe" style="max-width:100%;height:auto;border-radius:8px;margin:16px 0" /></p>
<h2>数字层面的进步</h2>
<p>按第三方机构Artificial Analysis的测量，Gemini 3.5 Transcribe在流式场景的平均词错误率（WER）是4.0%，非流式更低，只有2.6%；相比上一代Chirp 3，最终转写时间提升70%。FLEURS多语言基准上，词错误率5.04%，属于当前公开语音转写模型的头部水平。</p>
<p>语言支持覆盖85种以上，自动识别地区口音和方言；预录音频能区分最多3位说话人并给出时间戳。对中文用户来说，带口音的普通话、夹杂英文术语的会议、嘈杂环境里的录音，这些以前容易翻车的场景都是它优化的重点——官方说它在真实世界的嘈杂环境中表现稳定，还能准确抓取邮政编码、订单号这类字母数字实体。</p>
<h2>聪明的地方在&#8221;会整理&#8221;</h2>
<p>传统语音识别是把声音变成字，Gemini 3.5 Transcribe多做了两步&#8221;整理&#8221;：智能转写会自动处理说话人自我纠正（比如&#8221;周二见面——不对，周三&#8221;），去掉&#8221;嗯&#8221;&#8221;啊&#8221;这类填充词，并自动格式化文本；自定义词汇表能识别专业术语和独特拼写，医疗、法律、技术这类领域的词表可以直接喂给它。它还支持函数调用——转写过程中可以把图像生成、文件分析等子任务委托给其他Gemini模型。</p>
<h2>怎么用</h2>
<p>开发者有两条API：Live API做实时双向流式转写（亚秒级延迟，适合语音助手、实时字幕），Interactions API处理录音、会议、通话记录（带说话人归属和时间戳）。模型标识分别是gemini-3.5-transcribe-live和gemini-3.5-transcribe，今天起在Google AI Studio公开预览。</p>
<p>大众端也已经铺开：Gemini的macOS应用支持语音转写和结合屏幕上下文的语音操作，安卓的Gboard新增Rambler功能——说话直接变成格式良好的文字，还能用语音编辑、纠正拼写。Chrome里&#8221;边说话边打字&#8221;也快来了。</p>

---

原文链接：[https://www.hxsf.com.cn/geminidt/2605](https://www.hxsf.com.cn/geminidt/2605)
