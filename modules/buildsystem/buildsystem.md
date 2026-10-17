# buildsystem

状态：in-progress（按代码推断，2026-10-17）

## 做什么

构建系统、第三方依赖和 CI。

构建说明见 `docs/dev/BUILD.md`；第三方代码以 submodule 放在 `3rdparty/`，从源码构建。

## 代码在哪

- `CMakeLists.txt`
- `cmake/`
- `3rdparty/`
- `.gitmodules`
- `.github/workflows/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
