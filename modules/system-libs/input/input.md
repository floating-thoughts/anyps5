# input

状态：in-progress（按代码推断，2026-10-17）

## 做什么

输入设备：手柄、键鼠、输入法、USB/蓝牙、VR 头显、手势。

按键映射配置见 `docs/user/INPUT_MAPPING.md`。

## 代码在哪

- `core/libs/prx/libScePad/`
- `core/libs/prx/libSceMouse/`
- `core/libs/prx/libSceKeyboard/`
- `core/libs/prx/libSceConvertKeycode/`
- `core/libs/prx/libSceIme/`
- `core/libs/prx/libSceImeBackend/`
- `core/libs/prx/libSceBluetoothHid/`
- `core/libs/prx/libSceUsbd/`
- `core/libs/prx/libSceUsbStorage/`
- `core/libs/prx/libSceMbus/`
- `core/libs/prx/libSceHmd/`
- `core/libs/prx/libSceHmd2/`
- `core/libs/prx/libSceVrTracker2/`
- `core/libs/prx/libSceSystemGesture/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 129/195 个已声明函数已实现。

- `libScePad` 25/43
- `libSceMouse` 4/5
- `libSceKeyboard` 6/6
- `libSceConvertKeycode` 3/4
- `libSceIme` 13/14
- `libSceImeBackend`（无独立导出，共享其他库的源码或只有占位）
- `libSceBluetoothHid` 5/8
- `libSceUsbd` 40/40
- `libSceUsbStorage`（无独立导出，共享其他库的源码或只有占位）
- `libSceMbus` 4/4
- `libSceHmd` 9/9
- `libSceHmd2` 1/30
- `libSceVrTracker2` 0/10
- `libSceSystemGesture` 19/22

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
