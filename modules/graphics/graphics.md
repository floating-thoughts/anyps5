# graphics

状态：in-progress（按代码推断，2026-10-17）

## 做什么

GPU 相关系统库：AGC 命令缓冲、驱动（PM4 执行 + Vulkan 后端）、视频输出。

流程见 `docs/dev/ARCHITECTURE.md` 的 Graphics 一节：游戏命令缓冲 → libSceAgcDriver/Submit → Execution/Pm4 → 着色器缓存或 shader-recompiler → Vulkan 管线。

## 代码在哪

- `core/libs/prx/libSceAgc/`
- `core/libs/prx/libSceAgcDriver/`
- `core/libs/prx/libSceVideoOut/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
