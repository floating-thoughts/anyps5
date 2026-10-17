# dialogs

状态：in-progress（按代码推断，2026-10-17）

## 做什么

系统对话框：CommonDialog 和各类 *Dialog / Cdlg* 库。

## 代码在哪

- `core/libs/prx/libSceCommonDialog/`
- `core/libs/prx/libSceMsgDialog/`
- `core/libs/prx/libSceMsgDialog.native/`
- `core/libs/prx/libSceErrorDialog/`
- `core/libs/prx/libSceImeDialog/`
- `core/libs/prx/libSceLoginDialog/`
- `core/libs/prx/libSceNetCtlApDialog/`
- `core/libs/prx/libSceNpAuthAuthorizedAppDialog/`
- `core/libs/prx/libScePlayGoDialog/`
- `core/libs/prx/libScePlayerInvitationDialog/`
- `core/libs/prx/libScePlayerSelectionDialog/`
- `core/libs/prx/libSceSaveDataDialog/`
- `core/libs/prx/libSceSaveDataDialog.native/`
- `core/libs/prx/libSceSigninDialog/`
- `core/libs/prx/libSceUsbStorageDialog/`
- `core/libs/prx/libSceVrSetupDialog/`
- `core/libs/prx/libSceWebBrowserDialog/`
- `core/libs/prx/libSceCdlgG2P/`
- `core/libs/prx/libSceCdlgPlayerReview/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 124/127 个已声明函数已实现。

- `libSceCommonDialog` 2/2
- `libSceMsgDialog` 10/10
- `libSceMsgDialog.native` 10/10
- `libSceErrorDialog` 6/6
- `libSceImeDialog` 8/8
- `libSceLoginDialog` 7/7
- `libSceNetCtlApDialog` 7/7
- `libSceNpAuthAuthorizedAppDialog` 7/7
- `libScePlayGoDialog` 7/7
- `libScePlayerInvitationDialog` 7/7
- `libScePlayerSelectionDialog` 1/1
- `libSceSaveDataDialog` 8/8
- `libSceSaveDataDialog.native` 10/10
- `libSceSigninDialog` 7/7
- `libSceUsbStorageDialog`（无独立导出，共享其他库的源码或只有占位）
- `libSceVrSetupDialog` 6/6
- `libSceWebBrowserDialog` 7/10
- `libSceCdlgG2P` 7/7
- `libSceCdlgPlayerReview` 7/7

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
