# Gemini 视频理解升级：token 消耗最高降88%，长视频分析成本大降

> 原文链接：[https://www.hxsf.com.cn/geminidt/2610](https://www.hxsf.com.cn/geminidt/2610)

<p><a href="https://www.hxsf.com.cn/jiaocheng" target="_blank" rel="noopener">Gemini</a> 看视频的方式换了一套。以前是固定每秒抽一帧，把整段画面从头到尾机械过一遍。现在模型会先定位再看，结合推理决定哪些画面值得放大、用什么速度看。这套能力叫智能体视频理解，9月1日起在 Google AI Studio 和 Gemini Enterprise Agent Platform 上线。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190554_657212.png" alt="Gemini智能体视频理解"></p>
<p>对成本的影响比想象中直接。官方数据里，启用后 token 消耗最高降 88%，成本最高降 66%，准确率最高还能提升 7%。差距在长视频上尤其明显，10 分钟的教程到几个小时的讲座，视频越长省得越多。</p>
<p>省在哪一步，简单说就是不再全程匀速扫。需要确认高速动作的时候，模型会提高帧率回看，其余部分一带而过，只取任务真正需要的画面、声音和字幕。</p>
<p>能干的事，官方列了四类。亚秒级时刻检索，快速动作里转瞬即逝的变化，单帧抽样的老办法容易漏，现在能精准定位。长视频里大海捞针，几个小时的素材直接问问题，不用再烧几百万 token。异常检测，对感兴趣的时间窗口提高帧率复查。还有动作与物体计数，重复动作能准确跟踪，不同物体能数清。</p>
<p>对中文用户比较实用的场景，是把一小时培训录像提炼成要点、从长会议视频里找某段发言、给视频剪辑做定位。这些以前要么费 token 要么费人工，现在模型自己会挑重点看。</p>
<p>支持 Gemini 3.7 Flash、3.6 Flash、3.5 Flash-Lite 三款模型，API 调用时把视频处理的 processing 参数设为 agentic 即可。可以上传视频，也可以直接贴 YouTube 链接，Gemini 应用端后续会向所有用户开放。定价走标准 API，没有额外功能费。想在 Gemini 上做视频分析应用的开发者，这个能力现在就能接进自己的流程里试。</p>

---

原文链接：[https://www.hxsf.com.cn/geminidt/2610](https://www.hxsf.com.cn/geminidt/2610)
