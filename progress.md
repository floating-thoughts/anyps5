# AnyPS5 进度

与 `architecture.md` 的模块树同构。仓库原来没有 progress.md，下面的状态全部**按代码推断**（2026-10-17）：系统库的完成度来自 `tools/progress.py` 的统计（全部系统库 3232/3665 个已声明函数已实现，着色器 1166/1166），各模块的具体数字写在各自的 `modules/<路径>/<名字>.md` 里。整个项目仍在活跃开发，每个模块近 30 天都有提交，所以全部标 `in-progress`。

- **relinker** `in-progress`（按代码推断）
  - **cli** `in-progress`（按代码推断）
  - **pipeline** `in-progress`（按代码推断）
  - **elf-patcher** `in-progress`（按代码推断）
  - **io** `in-progress`（按代码推断）
  - **codegen** `in-progress`（按代码推断）
  - **wasm** `in-progress`（按代码推断）
- **nid** `in-progress`（按代码推断）
- **shader-recompiler** `in-progress`（按代码推断）
  - **rdna-decoder** `in-progress`（按代码推断）
  - **control-flow** `in-progress`（按代码推断）
  - **ir** `in-progress`（按代码推断）
  - **translation** `in-progress`（按代码推断）
  - **optimization** `in-progress`（按代码推断）
  - **spirv-backend** `in-progress`（按代码推断）
- **graphics** `in-progress`（按代码推断）
  - **agc** `in-progress`（按代码推断）
  - **agc-driver** `in-progress`（按代码推断）
    - **submit** `in-progress`（按代码推断）
    - **execution** `in-progress`（按代码推断）
    - **vulkan** `in-progress`（按代码推断）
  - **video-out** `in-progress`（按代码推断）
- **system-libs** `in-progress`（按代码推断）
  - **kernel** `in-progress`（按代码推断）
    - **threads-sync** `in-progress`（按代码推断）
    - **memory-modules** `in-progress`（按代码推断）
    - **file-io** `in-progress`（按代码推断）
    - **system-time** `in-progress`（按代码推断）
  - **libc** `in-progress`（按代码推断）
  - **audio** `in-progress`（按代码推断）
  - **media** `in-progress`（按代码推断）
  - **input** `in-progress`（按代码推断）
  - **network** `in-progress`（按代码推断）
  - **services** `in-progress`（按代码推断）
  - **dialogs** `in-progress`（按代码推断）
- **guest-tests** `in-progress`（按代码推断）
- **tools** `in-progress`（按代码推断）
  - **progress-report** `in-progress`（按代码推断）
  - **repo-checks** `in-progress`（按代码推断）
  - **dev-utilities** `in-progress`（按代码推断）
  - **hw-oracle** `in-progress`（按代码推断）
  - **release** `in-progress`（按代码推断）
- **web-converter** `in-progress`（按代码推断）
- **buildsystem** `in-progress`（按代码推断）

## 待问清单

按"先按推荐做，再记录"，下面这些切分和归类已按推荐方案做完，等 user 回来确认：

1. **系统库按功能分组，不按库一一建模块**：`core/libs/prx` 下有约 140 个库，一库一模块会让顶层失控。推荐：graphics（Agc、AgcDriver、AgcVsh、VideoOut）单独做顶层，其余按功能分成 system-libs 下的 kernel、libc、audio、media、input、network、services、dialogs。备选：按上游 `docs/dev/debt/` 的一库一文件再细分到库。
2. **libkernel 再分四个子模块**（threads-sync、memory-modules、file-io、system-time），按 `libkernel/` 的子目录切；libSceFiber / Ult / JobManager 归 threads-sync，libSceAmpr / Sysmodule 归 memory-modules，kernel_sys / kernel_web / ulobjmgr / Rtc / Random / RazorCpu / DbgThreadSanitizer 归 system-time。备选：kernel 不分子模块。
3. **拿不准的库归类**：libSceAcm 归 audio，libScePsml 归 media，libSceCesCs（字符编码转换）归 media，libSceMbus 归 input，libSceGameLiveStreaming / SharePlay / Remoteplay 归 network，libSceShare 归 services。
4. **core/Decoder（Jpeg / Png）并进 system-libs/media**，不单独做模块：只有 8 个文件，只给 JpegDec / PngDec 用。
5. **guest-tests 单独做顶层模块**：`core/libs/tests` 有约 385 个测试文件，跨所有系统库，独立于任何一个库。libSceAgcDriver 自带的 `tests/` 归 graphics/agc-driver。
6. **与上游规范冲突**：上游 `tools/check_conventions.py` 的 `notes-file` 规则禁止在 README / CONTRIBUTING / .github / docs/dev / docs/user 以外放 .md 文件（"Notes, investigation and agent files go in the pull request, not in the repository"）。本分支新加的 `architecture.md`、`progress.md`、`modules/**` 会被这条规则拦下。推荐：这些文件只留在 floating-thoughts 的 fork 里，向上游 boykopovar/AnyPS5 提 PR 的分支不要带上它们。备选：把它们挪到 `docs/dev/modules/` 下（仍可能被 doc 规则检查）。
7. **缺少 demand.md**：仓库里没有，按规矩只能由 user 写。
