# system-libs

状态：in-progress（按代码推断，2026-10-17）

## 做什么

除图形以外的 PS5 系统库（prx）的原生实现，各自编译成共享库。

每个库在 `core/libs/prx/<库名>/`，用 `APS5_VABI` 定义导出；未实现的导出调用 `NotImplemented_nid_no_patch`。上游按库记的技术债在 `docs/dev/debt/<库名>.md`。

## 代码在哪

- `core/libs/prx/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
