# vulkan

状态：in-progress（按代码推断，2026-10-17）

## 做什么

Vulkan 后端：管线、资源、guest 内存导入、多重采样、深度面。

CachedPipeline、GuestBufferMemory、MultisampleTarget、DepthSurface 等；内置着色器在 `Graphics/shaders/`。

## 代码在哪

- `core/libs/prx/libSceAgcDriver/Graphics/`
- `core/libs/prx/libSceAgcDriver/Resource/`
- `core/libs/prx/libSceAgcDriver/State/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
