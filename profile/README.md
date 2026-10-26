 <div align="center">
  <img src="https://avatars.githubusercontent.com/u/86964862?s=200&v=4" alt="Pollinations.ai" width="100"/>

  # Pollinations.ai

  **Open-source AI for people who make things.**

  A community-driven platform for building with generative AI. One unified API for text, images, video, audio, 3D, and embeddings.

  [![Stars](https://img.shields.io/github/stars/pollinations/pollinations?style=flat-square&logo=github&label=Stars)](https://github.com/pollinations/pollinations)
  [![License](https://img.shields.io/github/license/pollinations/pollinations?style=flat-square)](LICENSE)
  [![Discord](https://img.shields.io/discord/885844321461485618?style=flat-square&logo=discord&label=Discord&color=5865F2)](https://discord.gg/k9F7SyTgqn)

  [Website](https://pollinations.ai) · [Playground](https://pollinations.ai/play) · [Dashboard & API Keys](https://enter.pollinations.ai) · [API Docs](https://gen.pollinations.ai/docs) · [Discord](https://discord.gg/k9F7SyTgqn)
</div>

---

## 🚀 One API. Many possibilities.

[Pollinations.ai](https://pollinations.ai) is an open-source generative AI platform that gives developers and creators access to a wide range of AI models through a unified API.

Instead of integrating every model provider separately, use one API to generate content, build applications, and connect AI tools.

- 📝 **Text & reasoning** — chat, vision, tool calling, and structured outputs.
- 🖼️ **Image generation & editing** — create images from prompts and transform existing images.
- 🎬 **Video generation** — generate videos from text and supported image inputs.
- 🔊 **Audio** — text-to-speech and speech-to-text.
- 🧊 **3D generation** — create 3D assets with supported models.
- 🔢 **Embeddings** — power semantic search, retrieval, and similarity matching.
- 🎙️ **Real-time AI** — connect to supported real-time conversational models.
- 🤖 **Managed agents** — turn prompts, models, and tools into reusable AI agents.
- 🧰 **Developer tools** — use the CLI, SDK, MCP servers, and OpenAI-compatible APIs.
- 🌱 **Community ecosystem** — publish models, build applications, and participate in Quests.

Model availability, pricing, and capabilities change over time. Explore the [live model catalog](https://gen.pollinations.ai/models) for current information.

## ⚡ Quick start

### 1. Get an API key

Create an account and generate a key at [enter.pollinations.ai](https://enter.pollinations.ai/keys).

Set your key as an environment variable:

```bash
export POLLINATIONS_API_KEY="YOUR_API_KEY"
```

Keep secret keys private. For browser-based applications, use an appropriately restricted app key or [Connect User Wallets](https://gen.pollinations.ai/docs#tag/connect-user-wallets).

### 2. Generate an image

```bash
curl -H "Authorization: Bearer $POLLINATIONS_API_KEY" \
  "https://gen.pollinations.ai/image/a%20cat%20in%20space" \
  -o image.jpg
```

### 3. Generate text

Use the OpenAI-compatible Chat Completions API:

```bash
curl https://gen.pollinations.ai/v1/chat/completions \
  -H "Authorization: Bearer $POLLINATIONS_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "openai/gpt-5.4-nano",
    "messages": [
      {
        "role": "user",
        "content": "Explain quantum computing in two sentences."
      }
    ]
  }'
```

The model shown is an example. Check the [live model catalog](https://gen.pollinations.ai/models) for current availability and access requirements.

### 4. Explore more

- [Interactive Playground](https://pollinations.ai/play)
- [Full API Documentation](https://gen.pollinations.ai/docs)
- [Available Models](https://gen.pollinations.ai/models)
- [Dashboard, Keys & Credits](https://enter.pollinations.ai)

## 🧩 A unified API

The API is hosted at `https://gen.pollinations.ai`.

| Capability | Endpoint | Description |
|---|---|---|
| Text | `POST /v1/chat/completions` | OpenAI-compatible chat completions |
| Text & agents | `POST /v1/responses` | Responses API |
| Anthropic-compatible text | `POST /v1/messages` | Messages API |
| Images | `GET /image/{prompt}` | Generate an image from a prompt |
| Image generation | `POST /v1/images/generations` | OpenAI-compatible image generation |
| Image editing | `POST /v1/images/edits` | Edit supported image inputs |
| Video | `GET /video/{prompt}` | Generate video |
| Speech | `POST /v1/audio/speech` | Generate audio from text |
| Transcription | `POST /v1/audio/transcriptions` | Transcribe audio |
| Embeddings | `POST /v1/embeddings` | Create embeddings |
| 3D | `GET /3d/{prompt}` | Generate 3D assets |
| Model discovery | `GET /v1/models` | Discover available models |
| Real-time | `/v1/realtime` | Supported real-time connections |

See the [API reference](https://gen.pollinations.ai/docs) for request formats, parameters, supported models, and endpoint-specific requirements.

## 💻 Use your existing tools

### OpenAI SDK compatibility

Pollinations supports OpenAI-compatible integrations. In many applications, you can switch providers by changing the base URL and API key.

**Python**

```python
from openai import OpenAI
import os

client = OpenAI(
    base_url="https://gen.pollinations.ai/v1",
    api_key=os.environ["POLLINATIONS_API_KEY"],
)

response = client.chat.completions.create(
    model="openai/gpt-5.4-nano",
    messages=[
        {"role": "user", "content": "Hello, Pollinations!"}
    ],
)

print(response.choices[0].message.content)
```

**JavaScript / Node.js**

```javascript
import OpenAI from "openai";

const client = new OpenAI({
  baseURL: "https://gen.pollinations.ai/v1",
  apiKey: process.env.POLLINATIONS_API_KEY,
});

const response = await client.chat.completions.create({
  model: "openai/gpt-5.4-nano",
  messages: [
    { role: "user", content: "Hello, Pollinations!" },
  ],
});

console.log(response.choices[0].message.content);
```

Compatibility depends on the endpoint and capabilities supported by the selected model.

### Pollinations CLI

Generate content, discover models, and manage your account from the terminal.

```bash
# Run a command without a global installation
npx @pollinations/cli gen text \
  "Explain quantum tunneling in one sentence"

# Generate an image
npx @pollinations/cli gen image \
  "A cozy futuristic city at night" \
  --output city.png

# Install the CLI globally
npm install -g @pollinations/cli

# Authenticate and discover models
polli auth login
polli models
polli docs
```

See the [CLI documentation](https://gen.pollinations.ai/docs#tag/cli) and [CLI source code](packages/polli-cli).

### SDK

Use the [Pollinations SDK](packages/sdk/README.md) for supported JavaScript, browser, and React integrations.

### MCP servers

Connect AI assistants and other Model Context Protocol clients to Pollinations-hosted tools.

**Pollinations MCP endpoint:**

```text
https://gen.pollinations.ai/mcp/pollinations
```

Configure your MCP client to use the endpoint and provide your API key using the authentication method supported by that client.

Explore the [MCP documentation](https://gen.pollinations.ai/docs#tag/mcp-servers).

## 🔐 Authentication & usage

Manage your API keys and account through the [Pollinations dashboard](https://enter.pollinations.ai).

| Key type | Typical use |
|---|---|
| App key (`pk_`) | Browser, mobile, and other public-client integrations with configured permissions and budgets |
| Secret key (`sk_`) | Trusted server-side applications |

**Security guidelines**

- Never expose a secret key in frontend code, public repositories, or client-side bundles.
- Give each application only the permissions it needs.
- Configure model access and budgets for app keys.
- For user-funded applications, consider [Connect User Wallets](https://gen.pollinations.ai/docs#tag/connect-user-wallets), which allows users to authorize spending their own Pollen.

Pollinations uses Pollen credits for usage-based billing. Check the dashboard and live model catalog for current prices, limits, and access requirements rather than relying on static pricing examples.

## 🌍 Build with the community

### Community models

Connect supported model endpoints to Pollinations and use them through the unified API.

- Register and test your own model.
- Keep supported models private or publish them when eligible.
- Configure compatible fallback models where supported.
- Discover models and inspect health information.

Start with the [Publish a Model guide](https://gen.pollinations.ai/docs#tag/publish-a-model) and the [live model catalog](https://gen.pollinations.ai/v1/models).

### Managed agents

Create reusable agents using a system prompt, a base model, and supported tools.

Manage agents through the dashboard or CLI, and use their model IDs through the normal API.

See the [Publish an Agent guide](https://gen.pollinations.ai/docs#tag/publish-an-agent).

### Pollen Quests

Participate in community Quests and earn Pollen for eligible contributions and activities.

Explore current opportunities through the [dashboard](https://enter.pollinations.ai).

### Build an app

Have you created something with Pollinations? Share it with the community and submit it for consideration in the [app directory](https://pollinations.ai/apps).

## 🏗️ Project structure

This repository contains the platform's applications, APIs, packages, and supporting infrastructure.

| Directory | Purpose |
|---|---|
| [`pollinations.ai/`](pollinations.ai/) | Main website and frontend |
| [`gen.pollinations.ai/`](gen.pollinations.ai/) | Unified generation API and routing |
| [`enter.pollinations.ai/`](enter.pollinations.ai/) | Authentication, keys, and billing |
| [`shared/`](shared/) | Shared libraries, registries, and utilities |
| [`apps/`](apps/) | Community and platform applications |
| [`packages/`](packages/) | SDKs, CLI, MCP, and other packages |
| [`media.pollinations.ai/`](media.pollinations.ai/) | Media upload and delivery services |
| [`operations/`](operations/) | Infrastructure, operations, and monitoring |

For development setup, dependencies, and contribution instructions, see [DEVELOP.md](DEVELOP.md).

## 🤝 Contributing

Pollinations is built with the community. Contributions, bug reports, ideas, and applications are welcome.

- **Code:** Browse the repository and open a [pull request](https://github.com/pollinations/pollinations/pulls).
- **Bugs and ideas:** [Open an issue](https://github.com/pollinations/pollinations/issues).
- **Build an app:** Share your project through the [app submission process](https://github.com/pollinations/pollinations/issues/new?template=app-submission.yml).
- **Community:** Join our [Discord server](https://discord.gg/k9F7SyTgqn).
- **Development:** Read [DEVELOP.md](DEVELOP.md) before making changes.

## 💚 Support the project

The best way to support Pollinations is to build with it, share what you make, and contribute to the ecosystem.

You can also explore the project's [GitHub Sponsors](https://github.com/sponsors/pollinations) page.

## 📣 Stay connected

- [Website](https://pollinations.ai)
- [Dashboard & News](https://enter.pollinations.ai)
- [API Documentation](https://gen.pollinations.ai/docs)
- [Model Monitor](https://model-monitor.pollinations.ai)
- [GitHub](https://github.com/pollinations/pollinations)
- [Discord](https://discord.gg/k9F7SyTgqn)
- [X](https://x.com/pollinations_ai)
- [Instagram](https://instagram.com/pollinations_ai)
- [LinkedIn](https://www.linkedin.com/company/pollinations-ai)
- [Reddit](https://www.reddit.com/r/pollinations_ai/)
- [YouTube](https://www.youtube.com/c/pollinations)

## 📜 License

Pollinations is open-source software licensed under the [MIT License](LICENSE).

---

<div align="center">
  Made with ❤️ by the Pollinations community.
</div>
