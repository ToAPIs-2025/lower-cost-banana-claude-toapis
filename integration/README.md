# Banana Claude integration notes

This is an independent API asset example and integration contract. It is not an official upstream provider, and the contract JSON is not a validated upstream settings import. API output validation is separate from in-app acceptance.

Pinned upstream SHA: 6a2b1b51fdcc35932184f06e513646a6f6f4f7d8

- [skills/banana/scripts/banana_core.py](https://github.com/AgriciDaniel/banana-claude/blob/6a2b1b51fdcc35932184f06e513646a6f6f4f7d8/skills/banana/scripts/banana_core.py)
- [skills/banana/scripts/generate.py](https://github.com/AgriciDaniel/banana-claude/blob/6a2b1b51fdcc35932184f06e513646a6f6f4f7d8/skills/banana/scripts/generate.py)

Images: authenticate with Bearer, submit once and persist the id, poll the image generations/{id} route, and download result.data[0].url. Resolution fields differ by model; changing Base URL alone is insufficient.

No native video-model entry point was verified for this project. This example covers image assets only.

In-app checklist: model selection → duplicate-safe submission → task recovery → save originals → import/display in the original UI → reconcile billing. Full upstream UI acceptance remains pending.
