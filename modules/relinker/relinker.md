# relinker

状态：in-progress（按代码推断，2026-10-17）

## 做什么

把 PS5 ELF 转成 Linux ELF / Windows PE 的转换器（命令行程序 relinker）。

按 `core/relinker/main.cpp` 的顺序：可选的 `--to-intel` 指令降级 → RelinkerPipeline 按 NID 读导入、检查 syscall、过滤未用 NID、生成 SysV dynamic 段 → GuestModuleBuilder 转换游戏自带模块 → LinuxElfPatcher / WindowsPePatcher 输出。

## 代码在哪

- `core/relinker/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
