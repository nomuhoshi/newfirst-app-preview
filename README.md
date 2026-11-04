Test preview of 碎片编程 (NOT production). Built from nomuhoshi/newfirst-app integration commit eb11e25 + preview config 664614d.

## pr11/（#11 登录与同步测试入口，已接入 #41 修复和数据保护）
来自 newfirst-app 的集成分支 sonnet/11-integrated（#11 + #41 修复 + 数据保护 + 进度文件导出 + 存档修正，提交 3460331）。本地存储键前缀 `pr11:`、离线缓存前缀 `pr11-suipian-`，不读写正式版进度。真人验收步骤见 newfirst-app 的 docs/18-真人验收清单.md。

## pr11-design/（同上 + 新视觉“墨蓝立体电路 v2.1”）
来自 sonnet/11-integrated-design（提交 3349ed9（含地图路线连线、首屏压缩、进度文件导出））：在 pr11 的基础上叠加设计分支 sonnet/design-ink-3d。存储键前缀 `pr11design:`、缓存前缀 `pr11design-suipian-`，和 pr11/、正式版都互不读写。仅供试看，不是正式版。

## rc1/（正式版候选 rc-1 的独立预览，用于上线前验收）
来自 newfirst-app 的 `preview/rc-1`（源码与 `release/rc-1` 的 69168cf 相同，只多一个预览工作流），对应 Draft PR #42：U1–U5 全部关卡（34 关）、判题与代码题答题页（代码题仍“待开放”）、账号登录与云存档、数据保护、进度文件导出/导入。本地存储键前缀 `rc1:`、离线缓存前缀 `rc1-suipian-`，不读写正式版进度，也不和 `pr11/` 互相读写。不是正式版；新版墨蓝视觉不在内。
