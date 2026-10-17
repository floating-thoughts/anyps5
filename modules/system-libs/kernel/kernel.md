# kernel

状态：in-progress（按代码推断，2026-10-17）

## 做什么

libkernel 及相关运行时库：线程、内存、模块加载、文件、时间。

libkernel 由几块独立功能组成，所以再分四个子模块；这里的完成度是整个 libkernel 的。

## 代码在哪

- `core/libs/prx/libkernel/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 576/612 个已声明函数已实现。

- `libkernel` 576/612

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
