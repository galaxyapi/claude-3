# Claude-3 API ☁️

Meet **Claude 3 Haiku**, a speed demon that processes 30 pages in a blink, an intellect setting new benchmarks, and a visionary deciphering photos to technical diagrams. 
Perfect for **roleplaying** ✨

# Features 🌟
- Simple API (OpenAI)
- No Cost
- Easy Integration, suitable for any Frontend

# Requirements
- python3 or nodejs (Optional)
- openai (Optional)
- Galaxy API Key [get here](https://discord.com/invite/rDfeS6Jf) 🆓

# Front-End Integration
If you're using it through any front-end, 
for Librechats, Sillytavern, JanitorAI etc.

1. Replace the Proxy url to
```https://galaxyapi.onrender.com```
2. Put your own galaxy API Key 🔐
3. That's it!

# Examples

```bash
curl https://galaxyapi.onrender.com/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $GALAXYAI_API_KEY" \
  -d '{
    "model": "claude-3-haiku-20240307",
    "messages": [
      {
        "role": "system",
        "content": "You are a helpful assistant."
      },
      {
        "role": "user",
        "content": "Hello!"
      }
    ]
  }'
```
Python
```python
from openai import OpenAI
client = OpenAI(apikey="galaxy-secret-key-here")
client.base_url = "https://galaxyapi.onrender.com/v1"

completion = client.chat.completions.create(
  model="claude-3-haiku-20240307",
  messages=[
    {"role": "system", "content": "You are a helpful assistant."},
    {"role": "user", "content": "Hello!"}
  ]
)

print(completion.choices[0].message)
```

NodeJS

```js
import OpenAI from "openai";

const openai = new OpenAI({
  apiKey: 'GALAXY_API_KEY',
  baseURL: 'https://galaxyapi.onrender.com/v1'
})

async function main() {
  const completion = await openai.chat.completions.create({
    messages: [{ role: "system", content: "You are a helpful assistant." }],
    model: "claude-3-haiku-20240307",
  });

  console.log(completion.choices[0]);
}

main();
```
# ContactUS ✋
Having Issues, Feel free to report it by creating the issue or report it [here](https://discord.com/invite/rDfeS6Jf).
