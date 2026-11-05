Test preview of 碎片编程 (NOT production). Built from nomuhoshi/newfirst-app integration commit eb11e25 + preview config 664614d.

## pr11-design/（旧版墨蓝设计预览，云端已关闭）
来自 sonnet/11-integrated-design（提交 a34d15f）：旧的“墨蓝立体电路 v2.1”视觉 + #11 功能。**云端已关闭**（测试入口不连正式 Supabase，只能在本机学习），存储键前缀 `pr11design:`、缓存前缀 `pr11design-suipian-`。仅供试看视觉，不是正式版；新版墨蓝实验手账由另一条设计线实现。

## rc1/（正式版候选 rc-1 的独立预览，用于上线前验收）
来自 newfirst-app 的 `preview/rc-1`（源码 = `release/rc-1` 的 752dc85（云端关闭；换项目后同邮箱登录只加载新项目自己的进度，旧项目副本保留），只多预览工作流），对应 Draft PR #42：U1–U5 全部关卡（34 关）、判题与代码题答题页（代码题仍“待开放”）、账号登录与云存档、数据保护、进度文件导出/导入。存储键前缀 `rc1:`、缓存前缀 `rc1-suipian-`。**云端只连独立的测试 Supabase 项目；测试项目还没配置时云端关闭**（只能在本机学习），永远不连正式项目。配置方法见 newfirst-app 的 `docs/22-test-supabase-setup.md`。新版墨蓝视觉不在内。

## u6/（U6 前两关「类型与报错」的独立课程预览，产品官已审题）
来自 newfirst-app 的 `preview/u6-part1`（源码 = `content/u6-part1` 的 eb54daa，完整 CI 通过：build、Chromium、WebKit；只多预览工作流）：在 U1–U5 之后多出 U6「类型与报错」的前两关（U6L1 它是什么类型、U6L2 文字和数字互换），U7「字典」仍是“即将推出”。U6 其余四关还没做。存储键前缀 `u6:`、缓存前缀 `u6-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。


## ink-3d/（墨蓝实验手账 · 地图首屏与路线，独立设计预览）
来自 newfirst-app 的 `sonnet/design-ink-3d-1`（提交 a539935，基于 main 70cbb7d，不含 #42 的账号/云端功能，所以**没有云端**，只能在本机学习）：墨蓝深色立体视觉 + 关卡之间的路线连线 + 左右来回的蛇形节点 + 首屏压缩。存储键前缀 `ink3d:`、缓存前缀 `ink3d-suipian-`；浏览器不让装前缀时会停止运行，不碰正式站和其他预览的数据。rc1/、#42、正式站都没动。
