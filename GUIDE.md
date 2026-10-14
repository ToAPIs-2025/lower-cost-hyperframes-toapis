# Lower-cost Hyperframes product video

## Inputs

[Original prompts and parameters](cases/briefs.json)

## Generation and outputs

Three ToAPIs product images → Hyperframes HTML timeline → local MP4 rendering. Image API calls are charged; local rendering does not call a video model.

Run cases in order; preserve original PNGs and SHA256. Reference cases depend on the first output. Generate or reuse it first. Never remove private-state just to rerun a task.

## Reuse for your product

Replace the first product description and preserve subject constraints in both reference prompts. Copy outputs to assets/01-soap.png, 02-orchard.png and 03-bathroom.png. Edit titles, timing and colors in demo/index.html, then run lint, check and render. GSAP is local; there are no remote images/scripts, TTS, music or video model calls.

## Parameters and screenshots

[Exact request evidence](evidence/runs.json) · [Original outputs](assets/)

Bilingual overview cards use original outputs and sanitized request facts. They are not upstream UI screenshots.
