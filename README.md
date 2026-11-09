Test preview of 碎片编程 (NOT production). Built from nomuhoshi/newfirst-app integration commit eb11e25 + preview config 664614d.

## pr11-design/（旧版墨蓝设计预览，云端已关闭）
来自 sonnet/11-integrated-design（提交 a34d15f）：旧的“墨蓝立体电路 v2.1”视觉 + #11 功能。**云端已关闭**（测试入口不连正式 Supabase，只能在本机学习），存储键前缀 `pr11design:`、缓存前缀 `pr11design-suipian-`。仅供试看视觉，不是正式版；新版墨蓝实验手账由另一条设计线实现。

## rc1/（正式版候选 rc-1 的独立预览，用于上线前验收）
来自 newfirst-app 的 `preview/rc-1`（源码 = `release/rc-1` 的 752dc85（云端关闭；换项目后同邮箱登录只加载新项目自己的进度，旧项目副本保留），只多预览工作流），对应 Draft PR #42：U1–U5 全部关卡（34 关）、判题与代码题答题页（代码题仍“待开放”）、账号登录与云存档、数据保护、进度文件导出/导入。存储键前缀 `rc1:`、缓存前缀 `rc1-suipian-`。**云端只连独立的测试 Supabase 项目；测试项目还没配置时云端关闭**（只能在本机学习），永远不连正式项目。配置方法见 newfirst-app 的 `docs/22-test-supabase-setup.md`。新版墨蓝视觉不在内。

## u6/（U6 前五关「类型与报错」的独立课程预览）
来自 newfirst-app 的 `preview/u6-part1`（源码 = `content/u6-part3` 的 7f4028c，完整 CI 通过：build、Chromium、WebKit；只多预览工作流）：在 U1–U5 之后多出 U6「类型与报错」的前五关（它是什么类型、文字和数字互换、读懂报错、修正常见错误、用 print 找 bug），U7「字典」仍是“即将推出”。U6L6 项目「修好收银程序」已写好但**待开放**（它的代码题要等代码题运行器），不在地图上。含新题型“读报错选择题”。存储键前缀 `u6:`、缓存前缀 `u6-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。


## u7/（U7「字典」前五关的独立课程预览）
来自 newfirst-app 的 `preview/u7`（源码提交 68fbf31；完整 CI 在源码相同的 d96df6a 上通过：build、Chromium、WebKit；68fbf31 只多改了预览工作流的触发条件）= 课程分支 `preview/u6-part1`（U1–U6）+ U7 内容 + 空格修复（Draft PR #43：题面代码块保留缩进和空格）。U7「字典」5 关可玩（用键查值、更新已有的键、安全地查、新增与删除、遍历 `for name in stock`）；U7L6 库存小程序已写好但**待开放**（它的代码题要等代码题运行器），不在地图上。地图最后多一个“即将推出”的 U8 占位。存储键前缀 `u7:`、缓存前缀 `u7-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。rc1/、u6/、正式站都没动。


## u8/（U8「函数」前六关的独立课程预览）
来自 newfirst-app 的 `preview/u8`（源码提交 4ddddcc，即 CI 通过的提交本身；完整 CI：run 41992350816 第 1 次尝试，build、Chromium、WebKit 全部成功，deploy 按设计跳过；线上构建：run 41993535176）= U7 预览 `preview/u7`（U1–U7，含空格修复，Draft PR #43）+ U8「函数」前六关：定义和调用（def 只定义不运行、名字() 才是调用）、给函数一个参数、返回结果（return 与 print 的区别；函数执行结束时没有遇到 return，会自动返回 None；执行到 return 后本次调用就结束）、组合调用（返回的数字参与计算、f(g(x)) 先算里面）、两个参数和默认值（先教两个参数，再教默认值）、函数里的变量（在这些例子中，函数内定义的局部名字不能在函数外直接使用；给参数 price 重新赋值，不会改变外面的 price）。地图最后多一个“即将推出”的 U9「毕业小项目」占位；L7 价格计算器项目还没进预览。存储键前缀 `u8:`、缓存前缀 `u8-suipian-`。**云端关闭**（不连任何 Supabase，只能在本机学习），不是正式版，不并入 #42。rc1/、u6/、u7/、正式站都没动。

## access-check/（微信白屏 / 打不开 诊断页的独立预览，纯前端、只读）
来自 newfirst-app 的 `sonnet/access-test-verify`（提交 2ee5339，基于 release/rc-1 9d1b4cb，完整 CI 通过：build、Chromium、WebKit；诊断页专项测试 27/27）。入口：`access-check/access-test.html`。让对方点“开始测试”，等它跑完，点“复制结果”发回来。**页面只读：不连云端、不创建账号、不写数据**（诊断配置为空；即使手动加 `?cloud=1` 也因为没配置而不连）。存储键前缀 `accesscheck:`、缓存前缀 `accesscheck-suipian-`。同一台手机上请分别在微信和 Safari 里各测一次，保留两份报告对比。rc1/、#42、正式站都没动。


## fallback/（白屏兜底提示改版的独立预览，云端关闭）
来自 newfirst-app 的 `sonnet/blank-screen-copy`（提交 0a88cc9，基于 release/rc-1 9d1b4cb；完整 CI 通过：build、Chromium、WebKit）。默认页面正常启动，用来对比的只有“主脚本已下载但脚本出错”时的兜底提示：已捕获脚本解析 / 启动异常且首屏没渲染出来 → 标题“页面脚本出错，应用未能启动”，错误详情放在下方可复制；确认是资源下载失败 → 仍是“页面没有正常加载”+ 网络建议。故障场景在本地用 `scripts/repro-blank-screen.mjs` 复现验收（线上这个目录不注入故障）。存储键前缀 `fallback:`、缓存前缀 `fallback-suipian-`。**云端关闭**（不连任何 Supabase），不是正式版，不并入 #42。rc1/、正式站都没动。



## acc1/（登录／同步／保存的测试版验收预览，只连测试 Supabase）
来自 newfirst-app 的 `sonnet3/test-acceptance-prep`（源码提交 d284d54a924f31d88d751a8b2aa4c8d1a5a7d4dc，基线 claude/auth-cleanup-read-failures aedba6b；完整 CI：run 42454587738，build、Chromium、WebKit 全部成功，deploy 按设计跳过）。构建时严格校验：云端只能是测试项目 `tqdwhtrextqlmctkryyg`（suipian-test），配置错误构建即失败。“我的”页显示源码提交、测试云项目、最近同步状态（只显示，没有任何清数据按钮）。存储键前缀 `acc1:`、缓存前缀 `acc1-suipian-`。**不连正式 Supabase**；真机验收步骤见 newfirst-app 的 `docs/38-real-device-acceptance-table.md`。rc1/、u6/、u7/、u8/、正式站都没动。


## acc2/（登录／同步 AUTH-MAIL-02 验收预览，只连测试 Supabase）
来自 newfirst-app 的 `preview/acc2`（源码提交 4021ae3ece1eba805c8e0c7ec2da0acdd4f59713 = `fix/auth-mail-02`，基线 fix/auth-mail-01 4e2848e）。登录／同步错误提示按 DESIGN-AUTH-02（S1a–S6、V1–V4、C1）对齐：中文说明 + 诊断行 + 真实冷却时间 + “你的 XP 还在这台设备上”；多设备冲突不再是死路；游客进度选择可“稍后再说”（不自动覆盖云端）；键盘遮挡处理。继承 acc1 的存储隔离、源码提交显示、测试云项目校验。存储键前缀 `acc2:`、缓存前缀 `acc2-suipian-`。**只连测试项目 `tqdwhtrextqlmctkryyg`，不连正式 Supabase**；Supabase 自带发信仍可能发不出邮件（SMTP 未配置，见 docs/38-smtp-resend-setup.md）。rc1/、acc1/、u6/、u7/、u8/、正式站都没动。
