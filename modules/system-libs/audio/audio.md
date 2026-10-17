# audio

状态：in-progress（按代码推断，2026-10-17）

## 做什么

音频：AJM 解码、AudioOut/In、3D 音频、NGS2、Opus、语音聊天、TTS。

## 代码在哪

- `core/libs/prx/libSceAjm/`
- `core/libs/prx/libSceAjm.native/`
- `core/libs/prx/libSceAjmi/`
- `core/libs/prx/libSceAudio/`
- `core/libs/prx/libSceAudio3d/`
- `core/libs/prx/libSceAudioIn/`
- `core/libs/prx/libSceAudioOut/`
- `core/libs/prx/libSceAudioPropagation/`
- `core/libs/prx/libSceAudiodec/`
- `core/libs/prx/libSceAudiodec.native/`
- `core/libs/prx/libSceNgs2/`
- `core/libs/prx/libSceNgs2.native/`
- `core/libs/prx/libSceOpusCeltDec/`
- `core/libs/prx/libSceOpusDec/`
- `core/libs/prx/libSceVoice/`
- `core/libs/prx/libSceVoiceChat/`
- `core/libs/prx/libSceVoiceQoS/`
- `core/libs/prx/libSceProprietaryVoiceChatHelperPrx/`
- `core/libs/prx/libSceAcm/`
- `core/libs/prx/libSceTextToSpeech2/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 188/248 个已声明函数已实现。

- `libSceAjm`（无独立导出，共享其他库的源码或只有占位）
- `libSceAjm.native` 21/35
- `libSceAjmi`（无独立导出，共享其他库的源码或只有占位）
- `libSceAudio`（无独立导出，共享其他库的源码或只有占位）
- `libSceAudio3d` 13/13
- `libSceAudioIn` 4/8
- `libSceAudioOut` 35/48
- `libSceAudioPropagation` 22/23
- `libSceAudiodec` 6/6
- `libSceAudiodec.native`（无独立导出，共享其他库的源码或只有占位）
- `libSceNgs2`（无独立导出，共享其他库的源码或只有占位）
- `libSceNgs2.native` 35/38
- `libSceOpusCeltDec` 0/6
- `libSceOpusDec` 6/6
- `libSceVoice` 17/22
- `libSceVoiceChat` 8/8
- `libSceVoiceQoS` 2/14
- `libSceProprietaryVoiceChatHelperPrx` 3/4
- `libSceAcm` 8/9
- `libSceTextToSpeech2` 8/8

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
