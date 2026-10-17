# agc-driver

状态：in-progress（按代码推断，2026-10-17）

## 做什么

libSceAgcDriver：提交、执行命令缓冲并用 Vulkan 渲染。

测试在 `libSceAgcDriver/tests/`（约 430 个文件），工具在 `libSceAgcDriver/tools/`。

## 代码在哪

- `core/libs/prx/libSceAgcDriver/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 46/52 个已声明函数已实现。

- `libSceAgcDriver` 46/52

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
