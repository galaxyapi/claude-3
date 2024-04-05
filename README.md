# Free-claude-3 ☁️

Meet **Claude 3 Haiku**, a speed demon that processes 30 pages in a blink, an intellect setting new benchmarks, and a visionary deciphering photos to technical diagrams. 
Perfect for **roleplaying** ✨

# Features 🌟
- Simple API (OpenAI)
- No Cost
- Easy Integration, suitable for any Frontend

# Requirements
- python3 or nodejs
- openai
- Galaxy API Key [get here for free](https://discord.com/invite/rDfeS6Jf)

# Examples
Python
```python
from openai import OpenAI
client = OpenAI(apikey="galaxy-secret-key-here")
client.base_url = "https://galaxyapi.onrender.com"

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
```node
import OpenAI from "openai";

const openai = new OpenAI();
openai.base_url = "https://galaxyapi.onrender.com"

async function main() {
  const completion = await openai.chat.completions.create({
    messages: [{ role: "system", content: "You are a helpful assistant." }],
    model: "claude-3-haiku-20240307",
  });

  console.log(completion.choices[0]);
}

main();
```
