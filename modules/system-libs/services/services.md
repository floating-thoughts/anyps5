# services

状态：in-progress（按代码推断，2026-10-17）

## 做什么

系统服务：SystemService、UserService、存档、AppContent、PlayGo、更新、内容管理、分享。

## 代码在哪

- `core/libs/prx/libSceSystemService/`
- `core/libs/prx/libSceUserService/`
- `core/libs/prx/libSceSaveData/`
- `core/libs/prx/libSceSaveData.native/`
- `core/libs/prx/libSceAppContent/`
- `core/libs/prx/libScePlayGo/`
- `core/libs/prx/libSceGameUpdate/`
- `core/libs/prx/libSceContentDelete/`
- `core/libs/prx/libSceContentExport/`
- `core/libs/prx/libSceContentSearch/`
- `core/libs/prx/libSceShare/`
- `core/libs/prx/libSceShare.native/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 163/180 个已声明函数已实现。

- `libSceSystemService` 22/26
- `libSceUserService` 21/21
- `libSceSaveData` 9/9
- `libSceSaveData.native` 28/30
- `libSceAppContent` 13/14
- `libScePlayGo` 18/18
- `libSceGameUpdate` 6/7
- `libSceContentDelete` 2/4
- `libSceContentExport` 7/10
- `libSceContentSearch` 11/11
- `libSceShare` 17/17
- `libSceShare.native` 9/13

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
