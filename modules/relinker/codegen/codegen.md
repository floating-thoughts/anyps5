# codegen

状态：in-progress（按代码推断，2026-10-17）

## 做什么

`--to-intel`：把只有 AMD 支持的指令降级为 Intel 可执行的代码。

含 x86 指令长度解码器（`codegen/src/x86/X64InstructionDecoder.cpp`）。上游技术债：guest 模块 trampoline 只有合成测试覆盖。

## 代码在哪

- `core/relinker/codegen/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
