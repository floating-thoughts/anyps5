# system-time

状态：in-progress（按代码推断，2026-10-17）

## 做什么

系统信息、时间、kernel_sys / kernel_web、RTC、随机数、调试和性能工具库。

## 代码在哪

- `core/libs/prx/libkernel/System/`
- `core/libs/prx/libkernel/Time/`
- `core/libs/prx/libkernel_sys/`
- `core/libs/prx/libkernel_web/`
- `core/libs/prx/ulobjmgr/`
- `core/libs/prx/libSceRtc/`
- `core/libs/prx/libSceRandom/`
- `core/libs/prx/libSceRazorCpu/`
- `core/libs/prx/libSceDbgThreadSanitizer/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 59/66 个已声明函数已实现。

- `libkernel_sys` 11/16
- `libkernel_web`（无独立导出，共享其他库的源码或只有占位）
- `ulobjmgr` 2/2
- `libSceRtc` 34/34
- `libSceRandom` 1/1
- `libSceRazorCpu` 11/11
- `libSceDbgThreadSanitizer` 0/2

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
