# Lower-cost Banana Claude API asset examples

[English](README.md) · [中文](README_zh-CN.md)

Prepare image assets for Claude workflows.

October 16, 2026: 3 real images. Confirmed charge for these completed assets: **$0.0394 (7.88 credits)**, reconciled by task ID against the owner-provided dashboard export.

[ToAPIs · model pricing and setup](https://go2v.toapis.com/bc16ge)

## Examples

![Banana Claude image examples](screenshots/en/01-image-cases.png)

## Models and costs in this run

| Model | Preset | Catalog estimate / output | Settled charge |
|---|---|---:|---|
| gpt-image-2(VIP) | low / 1K | $0.0019 | $0.0019 |
| gpt-image-2.5-flare | high / 1K | $0.0225 | $0.0225 |
| Nano Banana 2.1 | 1K | $0.015 | $0.015 |

Catalog rates and confirmed charges match for these tested presets. Charges were reconciled against the owner-provided dashboard export at USD 0.005 per credit. Different models/presets do not imply equal quality. See evidence and examples for task records and originals.

## Run it

```bash
python -m pip install -r requirements.txt
python run_case.py --job jobs/gpt-image-2-vip.json
# Set TOAPIS_API_KEY privately in your local environment first.
python run_case.py --job jobs/gpt-image-2-vip.json --live
```

Dry-run by default. --live explicitly enables paid calls. Stable run_id values preserve task receipts; uncertain submissions are not automatically retried. Never commit .env, keys or private task state.

## Integrating with the original project

[Project-specific integration notes](integration/README.md) · [API contract](integration/toapis-contract.json)

[Banana Claude upstream](https://github.com/AgriciDaniel/banana-claude) · SHA `6a2b1b51fdcc35932184f06e513646a6f6f4f7d8`

These are original, independent ToAPIs asset/API examples, not an official upstream release or an accepted native provider. Full upstream UI, native registration and complete workflows still need maintainer acceptance. No upstream source is redistributed.
