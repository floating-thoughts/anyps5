# media

状态：in-progress（按代码推断，2026-10-17）

## 做什么

媒体和数据格式：视频解码、AvPlayer、JPEG/PNG 编解码、字体、zlib、XML/JSON、字符编码。

`core/Decoder/Jpeg`、`core/Decoder/Png` 是 JpegDec/PngDec 用到的独立解码器（各带测试）。

## 代码在哪

- `core/Decoder/`
- `core/libs/prx/libSceAvPlayer/`
- `core/libs/prx/libSceAvPlayer.native/`
- `core/libs/prx/libSceVideodec2/`
- `core/libs/prx/libSceVdecsw/`
- `core/libs/prx/libSceVideoRecordingP/`
- `core/libs/prx/libSceJpegDec/`
- `core/libs/prx/libSceJpegEnc/`
- `core/libs/prx/libScePngDec/`
- `core/libs/prx/libScePngEnc/`
- `core/libs/prx/libSceFont/`
- `core/libs/prx/libSceFont-module/`
- `core/libs/prx/libSceFont.native/`
- `core/libs/prx/libSceFontFt/`
- `core/libs/prx/libSceFontFt-module/`
- `core/libs/prx/libSceZlib/`
- `core/libs/prx/libSceXml/`
- `core/libs/prx/libSceJson2/`
- `core/libs/prx/libSceCesCs/`
- `core/libs/prx/libSceCesCs-module/`
- `core/libs/prx/libScePsml/`
- `core/libs/prx/libScePsml_debug/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 333/473 个已声明函数已实现。

- `libSceAvPlayer` 28/28
- `libSceAvPlayer.native`（无独立导出，共享其他库的源码或只有占位）
- `libSceVideodec2` 11/11
- `libSceVdecsw` 13/13
- `libSceVideoRecordingP` 2/9
- `libSceJpegDec` 5/5
- `libSceJpegEnc` 4/4
- `libScePngDec` 5/5
- `libScePngEnc` 4/4
- `libSceFont` 120/195
- `libSceFont-module`（无独立导出，共享其他库的源码或只有占位）
- `libSceFont.native`（无独立导出，共享其他库的源码或只有占位）
- `libSceFontFt` 23/42
- `libSceFontFt-module`（无独立导出，共享其他库的源码或只有占位）
- `libSceZlib` 5/5
- `libSceXml`（无独立导出，共享其他库的源码或只有占位）
- `libSceJson2` 104/116
- `libSceCesCs` 6/6
- `libSceCesCs-module`（无独立导出，共享其他库的源码或只有占位）
- `libScePsml`（无独立导出，共享其他库的源码或只有占位）
- `libScePsml_debug` 3/30

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
