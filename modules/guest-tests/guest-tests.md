# guest-tests

状态：in-progress（按代码推断，2026-10-17）

## 做什么

系统库的 guest 集成测试：用真实导入方式调用 prx 库，检查行为。

约 385 个测试源文件（Guest*.cpp 等），在 `core/libs/CMakeLists.txt` 里注册；注册是否齐全由 `tools/check_test_registration.py` 检查。

## 代码在哪

- `core/libs/tests/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
