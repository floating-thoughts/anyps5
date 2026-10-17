# network

状态：in-progress（按代码推断，2026-10-17）

## 做什么

网络和 PSN：Net、NetCtl、HTTP/HTTP2、SSL、RUDP、Np*、远程游玩、直播。

## 代码在哪

- `core/libs/prx/libSceNet/`
- `core/libs/prx/libSceNetCtl/`
- `core/libs/prx/libSceHttp/`
- `core/libs/prx/libSceHttp2/`
- `core/libs/prx/libSceSsl/`
- `core/libs/prx/libSceRudp/`
- `core/libs/prx/libSceNpAuth/`
- `core/libs/prx/libSceNpCommerce/`
- `core/libs/prx/libSceNpEntitlementAccess/`
- `core/libs/prx/libSceNpGameIntent/`
- `core/libs/prx/libSceNpManager/`
- `core/libs/prx/libSceNpPartner001/`
- `core/libs/prx/libSceNpSessionSignaling/`
- `core/libs/prx/libSceNpTrophy2/`
- `core/libs/prx/libSceNpUniversalDataSystem/`
- `core/libs/prx/libSceNpUtility/`
- `core/libs/prx/libSceNpWebApi2/`
- `core/libs/prx/libSceRemoteplay/`
- `core/libs/prx/libSceGameLiveStreaming/`
- `core/libs/prx/libSceSharePlay/`

## 当前状态

完成度来自 `tools/progress.py` 在 2026-10-17 的统计（已实现 / 已声明的导出函数）：合计 376/424 个已声明函数已实现。

- `libSceNet` 50/52
- `libSceNetCtl` 11/11
- `libSceHttp` 62/63
- `libSceHttp2` 36/43
- `libSceSsl` 8/28
- `libSceRudp` 20/24
- `libSceNpAuth` 10/10
- `libSceNpCommerce` 10/11
- `libSceNpEntitlementAccess` 21/21
- `libSceNpGameIntent` 4/4
- `libSceNpManager` 30/34
- `libSceNpPartner001` 2/2
- `libSceNpSessionSignaling` 13/17
- `libSceNpTrophy2` 17/18
- `libSceNpUniversalDataSystem` 41/41
- `libSceNpUtility` 5/5
- `libSceNpWebApi2` 26/29
- `libSceRemoteplay` 3/3
- `libSceGameLiveStreaming` 3/4
- `libSceSharePlay` 4/4

整个项目仍在活跃开发（近 30 天这一块有提交），所以标 in-progress。
