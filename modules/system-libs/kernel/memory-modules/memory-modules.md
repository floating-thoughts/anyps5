# memory-modules

状态：in-progress（按代码推断，2026-10-17）

## 做什么

直接内存、模块加载器、应用元数据、APR/AMM 命令缓冲、sysmodule。

Windows 延迟模块初始化（`DynamicLoader.cpp`）和 APR/AMM 设计见 `docs/dev/ARCHITECTURE.md`。

## 代码在哪

- `core/libs/prx/libkernel/DirectMemory/`
- `core/libs/prx/libkernel/Module/`
- `core/libs/prx/libkernel/AppMetadata/`
- `core/libs/prx/libkernel/Apr/`
- `core/libs/prx/libSceAmpr/`
- `core/libs/prx/libSceSysmodule/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 144/152 个已声明函数已实现。

- `libSceAmpr` 136/144
- `libSceSysmodule` 8/8

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
