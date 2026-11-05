Test preview of 碎片编程 (NOT production). Built from nomuhoshi/newfirst-app integration commit eb11e25 + preview config 664614d.

## pr11-design/（旧版墨蓝设计预览，云端已关闭）
来自 sonnet/11-integrated-design（提交 a34d15f）：旧的“墨蓝立体电路 v2.1”视觉 + #11 功能。**云端已关闭**（测试入口不连正式 Supabase，只能在本机学习），存储键前缀 `pr11design:`、缓存前缀 `pr11design-suipian-`。仅供试看视觉，不是正式版；新版墨蓝实验手账由另一条设计线实现。

## rc1/（正式版候选 rc-1 的独立预览，用于上线前验收）
来自 newfirst-app 的 `preview/rc-1`（源码 = `release/rc-1` 的 752dc85（云端关闭；换项目后同邮箱登录只加载新项目自己的进度，旧项目副本保留），只多预览工作流），对应 Draft PR #42：U1–U5 全部关卡（34 关）、判题与代码题答题页（代码题仍“待开放”）、账号登录与云存档、数据保护、进度文件导出/导入。存储键前缀 `rc1:`、缓存前缀 `rc1-suipian-`。**云端只连独立的测试 Supabase 项目；测试项目还没配置时云端关闭**（只能在本机学习），永远不连正式项目。配置方法见 newfirst-app 的 `docs/22-test-supabase-setup.md`。新版墨蓝视觉不在内。

## u6/（U6 前五关「类型与报错」的独立课程预览）
来自 newfirst-app 的 `preview/u6-part1`（源码 = `content/u6-part3` 的 7f4028c，完整 CI 通过：build、Chromium、WebKit；只多预览工作流）：在 U1–U5 之后多出 U6「类型与报错」的前五关（它是什么类型、文字和数字互换、读懂报错、修正常见错误、用 print 找 bug），U7「字典」仍是“即将推出”。U6L6 项目「修好收银程序」已写好但**待开放**（它的代码题要等代码题运行器），不在地图上。含新题型“读报错选择题”。存储键前缀 `u6:`、缓存前缀 `u6-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。


## u7/（U7「字典」前五关的独立课程预览）
来自 newfirst-app 的 `preview/u7`（源码提交 68fbf31；完整 CI 在源码相同的 d96df6a 上通过：build、Chromium、WebKit；68fbf31 只多改了预览工作流的触发条件）= 课程分支 `preview/u6-part1`（U1–U6）+ U7 内容 + 空格修复（Draft PR #43：题面代码块保留缩进和空格）。U7「字典」5 关可玩（用键查值、更新已有的键、安全地查、新增与删除、遍历 `for name in stock`）；U7L6 库存小程序已写好但**待开放**（它的代码题要等代码题运行器），不在地图上。地图最后多一个“即将推出”的 U8 占位。存储键前缀 `u7:`、缓存前缀 `u7-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。rc1/、u6/、正式站都没动。


## access-check/（微信白屏 / 打不开 诊断页的独立预览，纯前端、只读）
来自 newfirst-app 的 `sonnet/access-test-verify`（提交 2ee5339，基于 release/rc-1 9d1b4cb，完整 CI 通过：build、Chromium、WebKit；诊断页专项测试 27/27）。入口：`access-check/access-test.html`。让对方点“开始测试”，等它跑完，点“复制结果”发回来。**页面只读：不连云端、不创建账号、不写数据**（诊断配置为空；即使手动加 `?cloud=1` 也因为没配置而不连）。存储键前缀 `accesscheck:`、缓存前缀 `accesscheck-suipian-`。同一台手机上请分别在微信和 Safari 里各测一次，保留两份报告对比。rc1/、#42、正式站都没动。


## fallback/（白屏兜底提示改版的独立预览，云端关闭）
来自 newfirst-app 的 `sonnet/blank-screen-copy`（提交 0a88cc9，基于 release/rc-1 9d1b4cb；完整 CI 通过：build、Chromium、WebKit）。默认页面正常启动，用来对比的只有“主脚本已下载但脚本出错”时的兜底提示：已捕获脚本解析 / 启动异常且首屏没渲染出来 → 标题“页面脚本出错，应用未能启动”，错误详情放在下方可复制；确认是资源下载失败 → 仍是“页面没有正常加载”+ 网络建议。故障场景在本地用 `scripts/repro-blank-screen.mjs` 复现验收（线上这个目录不注入故障）。存储键前缀 `fallback:`、缓存前缀 `fallback-suipian-`。**云端关闭**（不连任何 Supabase），不是正式版，不并入 #42。rc1/、正式站都没动。

