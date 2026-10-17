# nid

状态：in-progress（按代码推断，2026-10-17）

## 做什么

NID 计算和 nid_patcher：构建后把系统库的导出改名为 NID。

NidCompute（SHA1）、NidResolver、ELF / PE / Mach-O 三种 NidPatcher、导出排除表。构建目标 `nid_patcher` 定义在 `core/libs/CMakeLists.txt`。

## 代码在哪

- `core/libs/nid/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
