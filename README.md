# GPT-5.6 Luna API (gpt-5.6-luna / gpt5.6luna) — llm guide with published pricing

> **input $0.16; cached_input $0.016; cache_write $0.2** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://apimart.ai/pricing)** · **[Get an API key](https://apimart.ai/keys)**

Everything here refers to **gpt-5.6-luna** — also written **gpt5.6luna** or **gpt 5.6 luna**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $0.16 |
| `cached_input` | $0.016 |
| `cache_write` | $0.2 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $16 |
| 1,000 | $160 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"gpt-5.6-luna","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
