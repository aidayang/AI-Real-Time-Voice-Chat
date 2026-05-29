# AI-Real-Time-Voice-Chat
一款AI实时语音聊天对话软件，Real-time AI voice chat conversations powered by ASR, LLM, and TTS

<img width="1910" height="911" alt="image" src="https://github.com/user-attachments/assets/27e24c43-3187-4b89-9f67-311e6ebb6350" />

AI 实时语音对话系统 是一款集语音识别（ASR）、大语言模型（LLM）对话、语音合成（TTS）于一体的实时语音交互软件。用户通过麦克风说话，系统自动识别语音内容并转为文字，交由 AI 角色进行智能回复，最终将回复内容合成为语音实时播放，实现端到端的自然语音对话体验。本来想测试英伟达的personaplex，但是发现personaplex不支持中文，一时兴起就做了当前这个软件。

### 全链路实时语音对话
语音输入 → 语音输出：用户只需点击录音按钮说话，系统自动完成”语音识别 → AI 推理 → 语音合成 → 语音播放”的完整闭环。

流式处理：ASR 文本、LLM 回复、TTS 音频均采用流式传输，AI 的思考过程和语音播报几乎同步呈现，延迟低、体验流畅。

WebSocket 实时通信：前后端通过 WebSocket 保持长连接，支持双向实时数据传输。

软件整个环节最耗时的为语音合成部分，依赖于显卡性能

### 注意事项
需要麦克风权限：首次使用时，浏览器会请求麦克风访问权限，请务必允许。

需要 LLM API Key：需用户自行在设置页面配置有效的 Base URL 和 API Key 方可使用对话功能。

网络要求：LLM 对话功能需要联网（调用远程 API）；ASR 和 TTS 可在本地运行。

性能建议：TTS 语音合成和 ASR 语音识别均消耗一定的 CPU/GPU 资源，建议英伟达显卡显存4G以上电脑使用。如遇卡顿，可适当提高音量阈值以减少不必要的音频处理。

扬声器回声：使用外放时，AI 回复的语音可能被麦克风重新拾取。建议佩戴耳机使用以获得最佳体验；软件也内置了”播报后静默期”机制来缓解此问题。

浏览器兼容：推荐使用 Chrome、Edge 等基于 Chromium 内核的现代浏览器，以确保 WebSocket 和 Web Audio API 的正常运行。

首次启动较慢：首次运行时会稍慢，请耐心等待。后续启动速度会明显加快。



### AI实时语音对话软件下载链接
### 本地TTS版：

https://pan.quark.cn/s/dfc1e9fa9784

### 云端TTS版：
上传中...
