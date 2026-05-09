# PoYo AI

One API for AI image, video, music, chat, and 3D models.

[Start building](https://poyo.ai) · [API docs](https://docs.poyo.ai) · [Create an API key](https://poyo.ai/dashboard/api-key) · [Models](https://poyo.ai/models) · [Pricing](https://poyo.ai/pricing) · [Examples](https://github.com/PoyoAPI/poyo-examples)

## Build With One API

PoYo AI gives developers a single API workflow for testing and shipping AI media features across leading model providers.

| Capability | What you can build |
| --- | --- |
| Image | Text-to-image, image editing, product visuals, creative tools |
| Video | Text-to-video, image-to-video, reference video workflows |
| Music | Music generation and audio workflows |
| Chat | Chat and text generation models |
| 3D | Text-to-3D and image-to-3D model workflows |

## Start Here

1. Create an account at [poyo.ai](https://poyo.ai).
2. Open the [API key dashboard](https://poyo.ai/dashboard/api-key).
3. Create an API key and store it server-side.
4. Submit a generation task with `POST https://api.poyo.ai/api/generate/submit`.
5. Save the returned `task_id`.
6. Poll status with `GET https://api.poyo.ai/api/generate/status/{task_id}`.
7. Use `callback_url` for production webhook delivery.

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
