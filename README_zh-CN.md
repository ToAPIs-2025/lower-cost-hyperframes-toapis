# 更低成本的 Hyperframes 产品短片方案


<!-- TOAPIS-MODELS-20261020 -->
## 模型与价格更新 · 2026-10-20

新增可独立运行的31套图片请求模板、8套视频模板。当前26套图片与8套视频可匹配同Key精确价格；另5套图片缺价，默认阻止新付费调用。它们属于额外API脚本；项目原生Provider、UI、导入及完整出片的验收范围仍以下方原教程为准。

| 图片模型／实测档位 | 当前档位报价／张 | 历史案例金额／张 | 费用证据 |
|---|---:|---:|---|
| gpt-image-2(VIP)<br><sub>low</sub> | $0.0019/image | **$0.0019/image** | 计费日志，阶段未知 |
| gpt-image-2.5-flare-vip<br><sub>low</sub> | 当前Key暂未返回报价 | **$0.005272/image**<br><sub>Token计费；当前$/M未返回，本例金额不是固定单张价。</sub> | 任务回执已结算 |
| nano_banana<br><sub>1K</sub> | $0.012/image | **$0.012/image** | 计费日志，阶段未知 |
| gemini-nano-banana-2.1<br><sub>1K</sub> | $0.015/image | **$0.015/image** | 计费日志，阶段未知 |
| gpt-image-2<br><sub>1K</sub> | $0.015/image | **$0.015/image** | 计费日志，阶段未知 |
| gemini-nano-banana-2.1-vip<br><sub>1K</sub> | $0.02/image | **$0.02/image** | 计费日志，阶段未知 |
| qwen-image-3.0<br><sub>1K</sub> | 当前Key暂未返回报价 | **$0.021/image** | 计费日志，阶段未知 |
| gpt-image-2.5-flare<br><sub>high</sub> | $0.0225/image | **$0.0225/image** | 计费日志，阶段未知 |
| gpt-image-2.5-sunburst<br><sub>high</sub> | $0.0225/image | **$0.0225/image** | 计费日志，阶段未知 |
| flux-2-pro<br><sub>1K</sub> | $0.025/image | **$0.025/image** | 计费日志，阶段未知 |
| doubao-seedream-5-0-pro<br><sub>1K</sub> | $0.042857/image | **$0.042856/image** | 计费日志，阶段未知 |

| 视频模型 | 档位／输入 | 本例消费 | 文件时长 | 本例每秒金额（升序） |
|---|---|---:|---:|---|
| MiniMax-H3-Max-Turbo | 5s / 480P / 文生视频 | $0.125/clip | 5.18s | **$0.024131/s**<br><sub>pricing底层费率：$0.025/s</sub> |
| seedance-2-mini | 4s / 480p / 首帧 | $0.13338/clip | 4.04s | **$0.033015/s**<br><sub>pricing底层费率：$3.285714/M total tokens</sub> |
| seedance-2-fast | 4s / 480p / 文生视频 | $0.214568/clip | 4.04s | **$0.053111/s**<br><sub>pricing底层费率：$5.285714/M total tokens</sub> |
| kling-v3 | 5s / 720p / std / 文生视频 | $0.3/clip | 5.04s | **$0.059524/s**<br><sub>pricing底层费率：$0.06/s</sub> |
| MiniMax-H3 | 5s / 768p / 文生视频 | $0.32/clip | 5.17s | **$0.061896/s**<br><sub>pricing底层费率：$0.064/s</sub> |
| seedance-2 | 4s / 480p / 首帧 | $0.26676/clip | 4.04s | **$0.06603/s**<br><sub>pricing底层费率：$6.571429/M total tokens</sub> |
| kling-3.0-turbo | 4s / 720p / 文生视频 | $0.32/clip | 4.04s | **$0.079208/s**<br><sub>pricing底层费率：$0.08/s</sub> |
| seedance-2-5 | 4s / 480p / 文生视频 | $0.3883/clip | 4.04s | **$0.096114/s**<br><sub>pricing底层费率：$10/M total tokens</sub> |

报价核对：2026-10-20。图片案例日期2026-10-17；视频案例日期2026-10-20。表格按本例金额／秒金额排序，质量、分辨率和输入不同，不是同配置质量排名。图片日志的阶段未知，不能当作单任务最终净结算；当前报价与历史金额分别显示。视频金额均由billing=settled确认，$/s按实际文件时长折算，任务处理耗时不参与计算。Token模型不是固定每秒价，底层$/M只作小字补充。

gpt-image-2(VIP)通用价格为$0.0019/image起；本例low/1K为$0.0019/image。新脚本有31套历史成功图片请求模板、8套视频模板；当前26套图片与8套视频可匹配价格，另5套图片因当前Key缺价而默认阻止新付费调用。

[本仓库多模型脚本](toapis-models/README_zh-CN.md) · [完整价表](PRICING_zh-CN.md) · [原图／视频及费用证据](https://github.com/ToAPIs-2025/toapis-quickstart/tree/main/tutorials/model-support-2026-10-20)

下方保留原项目历史案例、消费及集成说明；历史金额不改成今天的新报价。

<!-- /TOAPIS-MODELS-20261020 -->

<!-- TOAPIS-MODEL-COST-UPDATE-20261016 -->
## 模型类型、测试档位与花费

更新：2026-10-16。下表为已验证案例的历史档位与价格；本段补充不改变下方原批次记录。

| 模型（API ID） | 类型 | 测试档位 | 单次报价 | 已确认单次消费 | 数量 |
|---|---|---|---:|---:|---:|
| gpt-image-2(VIP) (`gpt-image-2-vip`) | 图片 | low / 1K / n=1 | $0.0019/image | $0.0019 | 3 |

原图片/视频案例已核对消费小计：**$0.0057**。

图片API及12秒本地MP4渲染已验证；本地渲染不是视频模型调用。

本地渲染不产生视频模型调用费用；不将图片消费除以12秒作为视频API价格。

gpt-image-2(VIP) **$0.0019/image 起**；本表 low/1K 实测档位为 **$0.0019/image**。不同模型、质量和分辨率不代表同质效果。
<!-- /TOAPIS-MODEL-COST-UPDATE-20261016 -->


[English](README.md)



以 ToAPIs `gpt-image-2-vip / low / 1K / n=1` 复用 Hyperframes 场景。3张 image-2(vip) 生图实扣 **$0.0057**。



ToAPIs 生成 3 张产品素材 → Hyperframes HTML 时间线 → 本地 MP4 渲染；图片 API 有费用，本地渲染不调用视频模型。



> 社区教程；未获上游背书。“更低成本”描述本次 API 档位，不表示整个软件或全部模型总成本更低。



## 演示



![API case overview](assets/overview-cn.png)



| 案例 | 原图 | 输出像素 |

|---|---|---|

| 01-soap | [PNG](assets/01-soap.png) | 1024 × 1024 |

| 02-orchard | [PNG](assets/02-orchard.png) | 1024 × 1024 |

| 03-bathroom | [PNG](assets/03-bathroom.png) | 1024 × 1024 |



### 视频演示



![12-second rendered demo](assets/product-preview.gif)



[MP4](assets/product-12s.mp4) · [HTML timeline](demo/index.html)



3 个场景 × 4 秒，1280×720、24 fps、无音轨；本地 Hyperframes 渲染，不是 ToAPIs 视频生成调用。



## 对应模型价格与本次花费



| Model | 配置 | API 单张报价 |

|---|---|---|

| `gpt-image-2-vip` | `low / 1K / n=1` | **$0.0019** |



3张 image-2(vip) 生图实扣 **$0.0057**。



[API pricing snapshot](evidence/pricing.json) · [Cost record](evidence/costs.json) · [Original requests](evidence/runs.json)



报价核查于 2026-10-14；不含其他画质、分辨率、模型、Agent 或机器成本。



[ToAPIs 模型落地页](https://go2v.toapis.com/1014_hyperframes_lowercost_gh_cn)



## 复现步骤



本机私有环境配置 `TOAPIS_API_KEY`，不要写进源码或聊天。`TOAPIS_BASE_URL=https://toapis.cn`（海外可用 `https://toapis.com`）。





```bash

# Inspect without paid calls

python scripts/run_demo.py

# Generate the original cases (charged; exact quote checked first)

python scripts/run_demo.py --live --output results

```



本通用脚本是独立 API 素材脚本；PPT Master 的原 CLI 实测记录单独标注在证据中。



```bash

cd demo

npm install

npx hyperframes lint

npx hyperframes check

npx hyperframes render --fps 24 --workers 1 --quality looks --output ../assets/product-12s.mp4

```



需 Node.js 22+、FFmpeg 与 Chromium；先把 results 的 3 张 PNG 复制到 assets 对应文件名。完整复用步骤见 [GUIDE](GUIDE_zh-CN.md)。



## 接口映射



```text

Authorization: Bearer TOAPIS_API_KEY

POST /v1/uploads/images             # reference PNG -> HTTPS URL

POST /v1/images/generations         # model,prompt,size,resolution,quality,n,reference_images

GET  /v1/images/generations/{id}    # poll the SAME task

completed -> result.data[0].url -> download PNG without the API key

```



生成 POST 不自动重试；轮询超时保留 `.toapis-state` 或 results/private-state 的任务 ID，重新执行同一用例会继续查询。参考改图不等于 mask 局部重绘；本轮没有测试 mask、透明背景、音频或云端视频。



## 上游与许可证



[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) · [pinned `d77b03c2`](https://github.com/heygen-com/hyperframes/tree/d77b03c24cd2e7c855c602fa8c4546f8076a1dca)



[Third-party notices](THIRD_PARTY_NOTICES.md)

