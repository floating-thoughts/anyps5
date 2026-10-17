# pipeline

状态：in-progress（按代码推断，2026-10-17）

## 做什么

核心转换流程：解析、分析、guest 模块、输出。

`relinker/src/` 下的 parsing、analysis、guest、pipeline、output；`domain/` 是共享的类型和接口（GuestRuntime、ImportModule、IProgress）。

## 代码在哪

- `core/relinker/relinker/`
- `core/relinker/domain/`

## 当前状态

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
