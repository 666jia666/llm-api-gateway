# llm-api-gateway
Unified API Gateway for DeepSeek, GLM, Qwen

# LLM API Gateway

**One unified API gateway for DeepSeek, GLM, and Qwen — accessible to developers outside China.**

---

## 🚀 Quick Start

**Base URL:** `http://144.202.122.105:6688/v1`

**Authentication:** Bearer Token

**Replace `YOUR_TOKEN` with your actual API key.**

### cURL

```bash
curl -X POST http://144.202.122.105:6688/v1/chat/completions \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "deepseek-v4-flash",
    "messages": [{"role": "user", "content": "Hello"}]
  }'
```

### Python

```python
import openai

openai.api_base = "http://144.202.122.105:6688/v1"
openai.api_key = "YOUR_TOKEN"

response = openai.ChatCompletion.create(
    model="deepseek-v4-flash",
    messages=[{"role": "user", "content": "Hello"}]
)

print(response["choices"][0]["message"]["content"])
```

### JavaScript (Node.js)

```javascript
const response = await fetch('http://144.202.122.105:6688/v1/chat/completions', {
  method: 'POST',
  headers: {
    'Authorization': 'Bearer YOUR_TOKEN',
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({
    model: 'deepseek-v4-flash',
    messages: [{'role': 'user', 'content': 'Hello'}]
  })
});

const data = await response.json();
console.log(data.choices[0].message.content);
```

### Expected Response

```json
{
  "choices": [{
    "message": {
      "role": "assistant",
      "content": "Hello! How can I help you today?"
    }
  }]
}
```

---

## 🧠 Available Models

| Model | Provider | Best For | Input (USD/1M) | Output (USD/1M) |
|-------|----------|----------|---------------|----------------|
| deepseek-v4-flash | DeepSeek | Everyday tasks, best value | $0.28 | $0.56 |
| deepseek-v4-pro | DeepSeek | Complex reasoning | $0.84 | $1.40 |
| glm-4-flash | Zhipu AI | Fast response, low cost | $0.14 | $0.42 |
| glm-5.1 | Zhipu AI | Coding, complex instructions | $1.40 | $3.92 |
| qwen-turbo | Tongyi Qwen | Lightweight, cost-effective | $0.11 | $0.34 |
| qwen-max | Tongyi Qwen | Long context, complex analysis | $2.10 | $7.00 |

---

## 💰 What $10 Gets You

| Model | Tokens for $10 |
|-------|----------------|
| qwen-turbo | ~30-90 million |
| glm-4-flash | ~24 million |
| deepseek-v4-flash | ~18-36 million |
| glm-5.1 | ~2.6-7.3 million |
| qwen-max | ~1.5-4.8 million |

*Typical conversation: ~500-1,000 tokens.*

---

## 💳 Payment

| Item | Details |
|------|---------|
| **Payment Method** | PayPal |
| **Minimum Top-up** | $10 |
| **How It Works** | I send you a PayPal invoice → you pay → I generate your API key within 30 minutes |

---

## 📁 Links

| Platform | Link |
|----------|------|
| **Discord** | https://discord.gg/9zVtyqVHJk |
| **Email** | 404321141@qq.com |
| **GitHub** | https://github.com/666jia666/llm-api-gateway |

---

## ❓ FAQ

| Question | Answer |
|----------|--------|
| **Do I need a Chinese phone number?** | No. PayPal is all you need. |
| **Do I need to sign a contract?** | No. Pay as you go, no commitment. |
| **What if my token runs out?** | Contact me for a new PayPal invoice to top up. |
| **Can I switch models?** | Yes — just change the `model` field in your request. |
| **Is there a free trial?** | Yes — ask me for a free trial token to test before you pay. |
| **What if I need help?** | Join the Discord server — I respond within 12 hours. |

---

**One API key. 6 models. $10 to start.**
