# libc

状态：in-progress（按代码推断，2026-10-17）

## 做什么

C / C++ 运行时：libc、libSceLibcInternal、POSIX for WebKit。

包括异常和栈展开（`libc/src/exception`）、各平台特定实现（`libc/src/specifics`）。

## 代码在哪

- `core/libs/prx/libc/`
- `core/libs/prx/libSceLibcInternal/`
- `core/libs/prx/libScePosixForWebKit/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 784/797 个已声明函数已实现。

- `libc` 748/759
- `libSceLibcInternal` 24/26
- `libScePosixForWebKit` 12/12

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
