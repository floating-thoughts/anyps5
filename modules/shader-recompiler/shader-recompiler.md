# shader-recompiler

状态：in-progress（按代码推断，2026-10-17）

## 做什么

把 PS5 的 RDNA 着色器重编译成 SPIR-V。

`Recompiler.cpp` 按 解码 → 控制流 → 翻译 → 优化 → SPIR-V 的顺序运行；开 `ANYPS5_ENABLE_SPIRV_TOOLS` 时再用 SPIRV-Tools 校验和优化。测试在 `core/shader/recompiler/tests/`。

## 代码在哪

- `core/shader/recompiler/`

## 当前状态

`tools/progress.py` 统计的着色器覆盖：1166/1166（100.0%）。

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
