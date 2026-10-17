# agc

状态：in-progress（按代码推断，2026-10-17）

## 做什么

libSceAgc：游戏侧构造命令缓冲（DCB/ACB）的 API。

子目录 Acb、Cb、Command、DcbDraw、DcbFlow、DcbState、Predication、Shader 等。

## 代码在哪

- `core/libs/prx/libSceAgc/`
- `core/libs/prx/libSceAgcVsh/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 206/229 个已声明函数已实现。

- `libSceAgc` 206/229
- `libSceAgcVsh`（无独立导出，共享其他库的源码或只有占位）

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
