# LLM API Gateway
Unified API Gateway for DeepSeek, GLM, Qwen

# LLM API Gateway

Unified API access to Chinese LLMs: DeepSeek, Zhipu GLM, Tongyi Qwen.

## Quick Start

```bash
curl -X POST http://144.202.122.105:6688/v1/chat/completions \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"model":"deepseek-v4-flash","messages":[{"role":"user","content":"Hello"}]}'
```

## Supported Models

| Model | Provider | Input Price (USD/1M) | Output Price (USD/1M) |
|-------|----------|---------------------|----------------------|
| deepseek-v4-flash | DeepSeek | $0.28 | $0.56 |
| deepseek-v4-pro | DeepSeek | $0.84 | $1.40 |
| glm-4-flash | Zhipu AI | $0.14 | $0.42 |
| glm-5.1 | Zhipu AI | $1.40 | $3.92 |
| qwen-turbo | Tongyi Qwen | $0.11 | $0.34 |
| qwen-max | Tongyi Qwen | $2.10 | $7.00 |

## $10 Gets You

| Model | Tokens you get for $10 |
|-------|------------------------|
| glm-4-flash | ~24 million |
| qwen-turbo | ~30-90 million |
| deepseek-v4-flash | ~18-36 million |
| glm-5.1 | ~2.6-7.3 million |
| qwen-max | ~1.5-4.8 million |

## Contact

- **Discord:** [Join our server](https://discord.gg/wtvo3dpoP)
- **Email:** 404321141@qq.com
