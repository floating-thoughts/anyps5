# threads-sync

状态：in-progress（按代码推断，2026-10-17）

## 做什么

线程和同步：pthread、取消、信号量、事件标志、equeue、fiber、ULT、job manager。

线程取消的设计见 `docs/dev/ARCHITECTURE.md` 的 Thread cancellation。libkernel 的完成度只在上一级 kernel 里统计（progress.py 不按子目录统计）。

## 代码在哪

- `core/libs/prx/libkernel/Pthread/`
- `core/libs/prx/libkernel/Semaphore/`
- `core/libs/prx/libkernel/EventFlag/`
- `core/libs/prx/libkernel/SyncOnAddress/`
- `core/libs/prx/libkernel/Equeue/`
- `core/libs/prx/libSceFiber/`
- `core/libs/prx/libSceUlt/`
- `core/libs/prx/libSceJobManager/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 61/64 个已声明函数已实现。

- `libSceFiber` 13/13
- `libSceUlt` 39/39
- `libSceJobManager` 9/12

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
