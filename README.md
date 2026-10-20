# Lower-cost Hyperframes product video


<!-- TOAPIS-MODELS-20261020 -->
## Model support and prices · 2026-10-20

Added standalone API presets: 31 image request templates and 8 video presets. Current-key pricing matches 26 image and 8 video presets; 5 image templates block new paid calls while pricing is unavailable. Native provider/UI/import/render acceptance remains as documented in the original guide below.

| Image model / tested preset | Current preset quote / image | Historical example amount / image | Fee evidence |
|---|---:|---:|---|
| gpt-image-2(VIP)<br><sub>low</sub> | $0.0019/image | **$0.0019/image** | Billing log, phase unknown |
| gpt-image-2.5-flare-vip<br><sub>low</sub> | Current-key quote unavailable | **$0.005272/image**<br><sub>Token-metered; current $/M unavailable. This sample is not a fixed image tariff.</sub> | Task receipt settled |
| nano_banana<br><sub>1K</sub> | $0.012/image | **$0.012/image** | Billing log, phase unknown |
| gemini-nano-banana-2.1<br><sub>1K</sub> | $0.015/image | **$0.015/image** | Billing log, phase unknown |
| gpt-image-2<br><sub>1K</sub> | $0.015/image | **$0.015/image** | Billing log, phase unknown |
| gemini-nano-banana-2.1-vip<br><sub>1K</sub> | $0.02/image | **$0.02/image** | Billing log, phase unknown |
| qwen-image-3.0<br><sub>1K</sub> | Current-key quote unavailable | **$0.021/image** | Billing log, phase unknown |
| gpt-image-2.5-flare<br><sub>high</sub> | $0.0225/image | **$0.0225/image** | Billing log, phase unknown |
| gpt-image-2.5-sunburst<br><sub>high</sub> | $0.0225/image | **$0.0225/image** | Billing log, phase unknown |
| flux-2-pro<br><sub>1K</sub> | $0.025/image | **$0.025/image** | Billing log, phase unknown |
| doubao-seedream-5-0-pro<br><sub>1K</sub> | $0.042857/image | **$0.042856/image** | Billing log, phase unknown |

| Video model | Preset / input | Settled clip charge | File duration | Case USD/s, ascending |
|---|---|---:|---:|---|
| MiniMax-H3-Max-Turbo | 5s / 480P / text-to-video | $0.125/clip | 5.18s | **$0.024131/s**<br><sub>Pricing tariff: $0.025/s</sub> |
| seedance-2-mini | 4s / 480p / first-frame | $0.13338/clip | 4.04s | **$0.033015/s**<br><sub>Pricing tariff: $3.285714/M total tokens</sub> |
| seedance-2-fast | 4s / 480p / text-to-video | $0.214568/clip | 4.04s | **$0.053111/s**<br><sub>Pricing tariff: $5.285714/M total tokens</sub> |
| kling-v3 | 5s / 720p / std / text-to-video | $0.3/clip | 5.04s | **$0.059524/s**<br><sub>Pricing tariff: $0.06/s</sub> |
| MiniMax-H3 | 5s / 768p / text-to-video | $0.32/clip | 5.17s | **$0.061896/s**<br><sub>Pricing tariff: $0.064/s</sub> |
| seedance-2 | 4s / 480p / first-frame | $0.26676/clip | 4.04s | **$0.06603/s**<br><sub>Pricing tariff: $6.571429/M total tokens</sub> |
| kling-3.0-turbo | 4s / 720p / text-to-video | $0.32/clip | 4.04s | **$0.079208/s**<br><sub>Pricing tariff: $0.08/s</sub> |
| seedance-2-5 | 4s / 480p / text-to-video | $0.3883/clip | 4.04s | **$0.096114/s**<br><sub>Pricing tariff: $10/M total tokens</sub> |

Pricing checked 2026-10-20. Image examples are dated 2026-10-17; video examples 2026-10-20. Tables sort by example amount or case USD/s. Presets and input modes differ; this is not a matched-settings quality ranking. Unknown-phase image logs are not confirmed final net settlements. Current quotes and historical amounts are separate. Video charges are billing=settled; case USD/s divides charge by actual file duration, never processing time. Token tariffs appear in small text and do not imply a fixed per-second price.

gpt-image-2(VIP) starts at $0.0019/image; this low/1K preset is $0.0019/image. The standalone sampler has 31 historically successful image request templates and 8 video presets. Current-key pricing matches 26 image and 8 video presets; 5 image templates block new paid submission until an exact price is available.

[Local sampler](toapis-models/README.md) · [Full price table](PRICING.md) · [Original media and fee evidence](https://github.com/ToAPIs-2025/toapis-quickstart/tree/main/tutorials/model-support-2026-10-20)

Original project examples, historical charges and integration instructions follow. Historical amounts are not rewritten as today’s quotes.

<!-- /TOAPIS-MODELS-20261020 -->

<!-- TOAPIS-MODEL-COST-UPDATE-20261016 -->
## Tested model types, presets and costs

Updated October 16, 2026. These are tested historical presets/prices; this addition does not relabel the original batch below.

| Model (API ID) | Type | Tested preset | Unit quote | Confirmed unit charge | Count |
|---|---|---|---:|---:|---:|
| gpt-image-2(VIP) (`gpt-image-2-vip`) | Image | low / 1K / n=1 | $0.0019/image | $0.0019 | 3 |

Confirmed original image/video example subtotal: **$0.0057**.

Image API calls and a 12-second local MP4 render validated; local rendering is not a video-model call.

Local rendering makes no video-model call. Dividing image spend by 12 seconds would not be a video API rate.

gpt-image-2(VIP), **from $0.0019/image**; the tested low/1K preset here is **$0.0019/image**. Different models, qualities and resolutions do not imply equivalent results.
<!-- /TOAPIS-MODEL-COST-UPDATE-20261016 -->


[中文](README_zh-CN.md)



ToAPIs `gpt-image-2-vip / low / 1K / n=1` for Hyperframes workflows. 3 image-2(vip) images: **$0.0057 actually charged**.



Three ToAPIs product images → Hyperframes HTML timeline → local MP4 rendering. Image API calls are charged; local rendering does not call a video model.



> Community tutorial; no upstream endorsement. “Lower-cost” describes this API tier, not total software or all-model costs.



## Demo



![API case overview](assets/overview-en.png)



| Case | Original image | Output pixels |

|---|---|---|

| 01-soap | [PNG](assets/01-soap.png) | 1024 × 1024 |

| 02-orchard | [PNG](assets/02-orchard.png) | 1024 × 1024 |

| 03-bathroom | [PNG](assets/03-bathroom.png) | 1024 × 1024 |



### Video demo



![12-second rendered demo](assets/product-preview.gif)



[MP4](assets/product-12s.mp4) · [HTML timeline](demo/index.html)



3 scenes × 4 seconds; 1280×720, 24 fps, no audio. Local Hyperframes rendering, not a ToAPIs video generation call.



## Model price and this demo’s cost



| Model | Configuration | API unit quote |

|---|---|---|

| `gpt-image-2-vip` | `low / 1K / n=1` | **$0.0019** |



3 image-2(vip) images: **$0.0057 actually charged**。



[API pricing snapshot](evidence/pricing.json) · [Cost record](evidence/costs.json) · [Original requests](evidence/runs.json)



Quote checked on 2026-10-14. Other tiers, resolutions, models, agents and machine costs are excluded.



[ToAPIs model landing page](https://go2v.toapis.com/1014_hyperframes_lowercost_gh_en)



## Reproduce



Set `TOAPIS_API_KEY` privately in your local environment. Keep it out of source code and chats. Use `TOAPIS_BASE_URL=https://toapis.cn` or `https://toapis.com`.





```bash

# Inspect without paid calls

python scripts/run_demo.py

# Generate the original cases (charged; exact quote checked first)

python scripts/run_demo.py --live --output results

```



The generic script is an external asset runner. Original PPT Master CLI runs are separately identified in the evidence.



```bash

cd demo

npm install

npx hyperframes lint

npx hyperframes check

npx hyperframes render --fps 24 --workers 1 --quality looks --output ../assets/product-12s.mp4

```



Requires Node.js 22+, FFmpeg and Chromium. First copy the 3 result PNGs to matching assets filenames. Full steps: [GUIDE](GUIDE.md).



## API mapping



```text

Authorization: Bearer TOAPIS_API_KEY

POST /v1/uploads/images             # reference PNG -> HTTPS URL

POST /v1/images/generations         # model,prompt,size,resolution,quality,n,reference_images

GET  /v1/images/generations/{id}    # poll the SAME task

completed -> result.data[0].url -> download PNG without the API key

```



Generation POST is never automatically retried. Preserve .toapis-state or results/private-state to resume the same task. Reference editing is not masked inpainting. Masks, transparency, audio and cloud video were not tested.



## Upstream and licenses



[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) · [pinned `d77b03c2`](https://github.com/heygen-com/hyperframes/tree/d77b03c24cd2e7c855c602fa8c4546f8076a1dca)



[Third-party notices](THIRD_PARTY_NOTICES.md)

