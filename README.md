Test preview of 碎片编程 (NOT production). Built from nomuhoshi/newfirst-app integration commit eb11e25 + preview config 664614d.

## pr11-design/（旧版墨蓝设计预览，云端已关闭）
来自 sonnet/11-integrated-design（提交 a34d15f）：旧的“墨蓝立体电路 v2.1”视觉 + #11 功能。**云端已关闭**（测试入口不连正式 Supabase，只能在本机学习），存储键前缀 `pr11design:`、缓存前缀 `pr11design-suipian-`。仅供试看视觉，不是正式版；新版墨蓝实验手账由另一条设计线实现。

## rc1/（正式版候选 rc-1 的独立预览，用于上线前验收）
来自 newfirst-app 的 `preview/rc-1`（源码 = `release/rc-1` 的 752dc85（云端关闭；换项目后同邮箱登录只加载新项目自己的进度，旧项目副本保留），只多预览工作流），对应 Draft PR #42：U1–U5 全部关卡（34 关）、判题与代码题答题页（代码题仍“待开放”）、账号登录与云存档、数据保护、进度文件导出/导入。存储键前缀 `rc1:`、缓存前缀 `rc1-suipian-`。**云端只连独立的测试 Supabase 项目；测试项目还没配置时云端关闭**（只能在本机学习），永远不连正式项目。配置方法见 newfirst-app 的 `docs/22-test-supabase-setup.md`。新版墨蓝视觉不在内。

## u6/（U6 前五关「类型与报错」的独立课程预览）
来自 newfirst-app 的 `preview/u6-part1`（源码 = `content/u6-part3` 的 7f4028c，完整 CI 通过：build、Chromium、WebKit；只多预览工作流）：在 U1–U5 之后多出 U6「类型与报错」的前五关（它是什么类型、文字和数字互换、读懂报错、修正常见错误、用 print 找 bug），U7「字典」仍是“即将推出”。U6L6 项目「修好收银程序」已写好但**待开放**（它的代码题要等代码题运行器），不在地图上。含新题型“读报错选择题”。存储键前缀 `u6:`、缓存前缀 `u6-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。
