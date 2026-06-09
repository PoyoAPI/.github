<p align="center">
  <a href="https://poyo.ai">
    <img src="./assets/header.svg" alt="PoYo AI - One API for AI model workflows" />
  </a>
</p>

<p align="center">
  <a href="https://poyo.ai"><img src="https://img.shields.io/badge/Start%20building-poyo.ai-84cc16?style=for-the-badge" alt="Start building" /></a>
  <a href="https://docs.poyo.ai"><img src="https://img.shields.io/badge/API%20docs-docs.poyo.ai-22d3ee?style=for-the-badge" alt="API docs" /></a>
  <a href="https://poyo.ai/models"><img src="https://img.shields.io/badge/Models-poyo.ai%2Fmodels-a78bfa?style=for-the-badge" alt="Models" /></a>
  <a href="https://github.com/PoyoAPI/poyo-examples"><img src="https://img.shields.io/badge/Examples-GitHub-111827?style=for-the-badge&logo=github" alt="Examples" /></a>
</p>

## One API for AI model workflows

PoYo AI gives developers one production API workflow for image, video, music, chat, and 3D model generation: submit a task, store `task_id`, poll in testing, and use webhooks in production.

Start with [PoyoAPI/poyo-examples](https://github.com/PoyoAPI/poyo-examples) for the full backend-safe workflow, then use focused model repos when you already know which model you want to integrate.

## Main examples repo

Use [PoyoAPI/poyo-examples](https://github.com/PoyoAPI/poyo-examples) when you want the full backend-safe path across cURL, Node.js, Python, Next.js routes, status polling, and production webhooks.

## Focused model repos

Use these when you already know the model you want and need a smaller repo to copy from.

| Category | Repository |
| --- | --- |
| Image | [gpt-image-2-api](https://github.com/PoyoAPI/gpt-image-2-api), [nano-banana-2-api](https://github.com/PoyoAPI/nano-banana-2-api), [nano-banana-pro-api](https://github.com/PoyoAPI/nano-banana-pro-api) |
| Video | [seedance-2-api](https://github.com/PoyoAPI/seedance-2-api), [sora-2-official-api](https://github.com/PoyoAPI/sora-2-official-api), [happy-horse-api](https://github.com/PoyoAPI/happy-horse-api) |

## Example model families

| Category | Families |
| --- | --- |
| Chat | ![Claude](https://img.shields.io/badge/Claude-111827?style=flat-square) ![GPT](https://img.shields.io/badge/GPT-0f172a?style=flat-square) ![Gemini](https://img.shields.io/badge/Gemini-2563eb?style=flat-square) |
| Image | ![GPT Image](https://img.shields.io/badge/GPT%20Image-111827?style=flat-square) ![FLUX](https://img.shields.io/badge/FLUX-ec4899?style=flat-square) ![Seedream](https://img.shields.io/badge/Seedream-10b981?style=flat-square) ![Nano Banana](https://img.shields.io/badge/Nano%20Banana-facc15?style=flat-square&labelColor=111827) |
| Video | ![Sora](https://img.shields.io/badge/Sora-111827?style=flat-square) ![Veo](https://img.shields.io/badge/Veo-2563eb?style=flat-square) ![Seedance](https://img.shields.io/badge/Seedance-06b6d4?style=flat-square) ![Kling](https://img.shields.io/badge/Kling-4f46e5?style=flat-square) ![Wan](https://img.shields.io/badge/Wan-7c3aed?style=flat-square) |
| Music | ![Suno](https://img.shields.io/badge/Suno-111827?style=flat-square) ![MiniMax Music](https://img.shields.io/badge/MiniMax%20Music-f97316?style=flat-square) |
| 3D | ![Meshy](https://img.shields.io/badge/Meshy-84cc16?style=flat-square&labelColor=111827) ![Tripo](https://img.shields.io/badge/Tripo-a78bfa?style=flat-square) |

## Quickstart

1. Create an account at [poyo.ai](https://poyo.ai).
2. Create an API key in the [dashboard](https://poyo.ai/dashboard/api-key).
3. Submit a generation task.
4. Save the returned `task_id`.
5. Poll status in testing.
6. Use `callback_url` webhooks in production.

```bash
export POYO_API_KEY="your-api-key"
export POYO_BASE_URL="https://api.poyo.ai"

curl -X POST "$POYO_BASE_URL/api/generate/submit" \
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

## Developer resources

- Website: [poyo.ai](https://poyo.ai)
- API docs: [docs.poyo.ai](https://docs.poyo.ai)
- Models: [poyo.ai/models](https://poyo.ai/models)
- API keys: [poyo.ai/dashboard/api-key](https://poyo.ai/dashboard/api-key)
- Examples: [PoyoAPI/poyo-examples](https://github.com/PoyoAPI/poyo-examples)
- Support: [support@poyo.ai](mailto:support@poyo.ai)
