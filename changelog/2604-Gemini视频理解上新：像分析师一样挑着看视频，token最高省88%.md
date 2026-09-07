# Gemini视频理解上新：像分析师一样挑着看视频，token最高省88%

> 原文链接：[https://www.hxsf.com.cn/geminidt/2604](https://www.hxsf.com.cn/geminidt/2604)

<p>9月1日，谷歌给Gemini的视频理解能力做了一次重要升级：推出agentic video understanding（智能体视频理解）。核心变化一句话讲清——以前AI看视频是&#8221;逐帧扫&#8221;，现在它会像分析师一样&#8221;挑着看&#8221;，先定位再放大，该省的全省了。</p>
<p><img decoding="async" src="https://cdn.laoshoucun.com/web/gemini/2026/09/20260904190554_657212.png" alt="Gemini智能体视频理解" style="max-width:100%;height:auto;border-radius:8px;margin:16px 0" /></p>
<h2>省到什么程度</h2>
<p>按官方数据：相比传统固定帧率处理，启用agentic视频理解后，token消耗最高降低88%，成本最高降低66%，准确率最高还能提升7%。效率提升在长视频上尤其明显——从10分钟的<a href="https://www.hxsf.com.cn/jiaocheng" target="_blank" rel="noopener">教程</a>视频，到90分钟的讲座、几个小时的活动录像，差距会越拉越大。</p>
<p>原理上，以前的静态处理是让模型按固定帧率（默认每秒1帧）把整段视频机械地吞进去；现在的做法是让模型结合推理和原生视频工具，动态决定看什么、看多快、用哪种模态看——需要确认高速动作时提高帧率重看，不需要的地方一带而过，全程只取任务需要的画面、声音和字幕。</p>
<h2>能干什么活</h2>
<p>官方给了四类典型能力：亚秒级时刻检索（精准定位转瞬即逝的画面变化，1帧率下容易漏掉）；长视频&#8221;大海捞针&#8221;搜索（数小时的视频里回答复杂问题，不用烧几百万token）；异常检测（对感兴趣的时间窗口提高帧率复查）；动作与物体计数（准确跟踪重复动作和数清不同物体）。</p>
<p>对中文用户来说，比较实用的场景包括：把一小时的培训录像快速提炼成要点、从长会议视频里精准找到某段发言、给视频做自动化剪辑定位。这些以前要么费token要么费人工，现在模型自己会&#8221;挑重点看&#8221;了。</p>
<h2>现在就能用</h2>
<p>Gemini 3.7 Flash、3.6 Flash和3.5 Flash-Lite三款模型都支持，API调用时把视频处理的processing参数设为agentic即可。今天起在Google AI Studio和Gemini Enterprise Agent Platform上线，支持上传视频和YouTube链接；Gemini应用端即将向所有用户开放。走的是标准API定价，没有额外功能费。</p>
<p>对开发者来说，这意味着&#8221;让AI看懂视频&#8221;的开发和算力成本同时降了一截。想在Gemini上做视频分析类应用的，这个更新值得第一时间接进来试。</p>

---

原文链接：[https://www.hxsf.com.cn/geminidt/2604](https://www.hxsf.com.cn/geminidt/2604)
