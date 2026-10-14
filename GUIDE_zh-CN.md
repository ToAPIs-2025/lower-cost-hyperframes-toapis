# 更低成本的 Hyperframes 产品短片方案

## 输入

[Original prompts and parameters](cases/briefs.json)

## 生成与输出

ToAPIs 生成 3 张产品素材 → Hyperframes HTML 时间线 → 本地 MP4 渲染；图片 API 有费用，本地渲染不调用视频模型。

逐案例执行；生成后保存原 PNG 与 SHA256。参考案例依赖首张图；先生成或复用首张图，再执行参考编辑。不要删除 private-state 后重跑同一任务。

## 复用到自己的产品

把 cases/briefs.json 的首图商品改成你的商品描述，两个参考编辑 prompt 保留主体约束。复制输出到 assets/01-soap.png、02-orchard.png、03-bathroom.png，按 demo/index.html 改标题、场景持续时间与颜色，再运行 lint、check、render。字体与 GSAP 均本地；不使用在线图片或远程脚本；没有 TTS、音乐或视频模型调用。

## 参数与截图

[Exact request evidence](evidence/runs.json) · [Original outputs](assets/)

README 中的双语封面由原图与脱敏请求信息制作，不是上游软件 UI 截图。
