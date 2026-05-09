<p align="center">
  <a href="https://poyo.ai">
    <img src="https://storage.poyo.ai/logo.webp" alt="PoYo AI" width="96" />
  </a>
</p>

<p align="center">
  <a href="https://poyo.ai"><img src="https://img.shields.io/badge/Get%20Started-poyo.ai-111111?style=for-the-badge" alt="Get Started" /></a>
  <a href="https://docs.poyo.ai"><img src="https://img.shields.io/badge/API%20Docs-docs.poyo.ai-2563eb?style=for-the-badge" alt="API Docs" /></a>
  <a href="https://poyo.ai/models"><img src="https://img.shields.io/badge/All%20Models-poyo.ai%2Fmodels-16a34a?style=for-the-badge" alt="All Models" /></a>
  <a href="https://github.com/PoyoAPI/poyo-examples"><img src="https://img.shields.io/badge/Examples-GitHub-0f172a?style=for-the-badge&logo=github" alt="Examples" /></a>
</p>

<p align="center">
  <a href="https://poyo.ai"><img src="https://img.shields.io/badge/Website-poyo.ai-f97316?style=flat-square" alt="Website" /></a>
  <a href="https://x.com/poyo_ai20351"><img src="https://img.shields.io/badge/X-PoYo%20AI-000000?style=flat-square&logo=x" alt="X" /></a>
  <a href="mailto:support@poyo.ai"><img src="https://img.shields.io/badge/Email-support%40poyo.ai-64748b?style=flat-square" alt="Email" /></a>
</p>

---

## One API for AI media models

PoYo AI helps developers build with image, video, music, chat, and 3D models through one API instead of stitching together provider-by-provider auth, billing, status polling, and webhook logic.

## Model coverage

| Category | Example model families |
| --- | --- |
| Chat | GPT · Claude · Gemini |
| Image | GPT Image · Seedream · Flux · Nano Banana |
| Video | Sora · Veo · Seedance · Kling · Wan |
| Music | Suno · MiniMax Music |
| 3D | Meshy · Tripo |

## Start here

- Website: [https://poyo.ai](https://poyo.ai)
- Docs: [https://docs.poyo.ai](https://docs.poyo.ai)
- Models: [https://poyo.ai/models](https://poyo.ai/models)
- API keys: [https://poyo.ai/dashboard/api-key](https://poyo.ai/dashboard/api-key)
- Examples: [https://github.com/PoyoAPI/poyo-examples](https://github.com/PoyoAPI/poyo-examples)

## Quickstart

```bash
curl -X POST "https://api.poyo.ai/api/generate/submit" \
  -H "Authorization: Bearer $POYO_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-image-2",
    "input": {
      "prompt": "A clean product render of a translucent AI cube on a white studio surface",
      "size": "1:1",
      "resolution": "1K",
      "quality": "low",
      "n": 1
    }
  }'
```

## Why teams use PoYo AI

- One API surface for image, video, music, chat, and 3D models
- Cleaner path from testing to production integration
- Shared task submission, polling, and webhook patterns
- One developer-facing workflow for model discovery and API keys

---

Built by the PoYo AI team · [poyo.ai](https://poyo.ai) · [support@poyo.ai](mailto:support@poyo.ai)
