<div align="center">
  <img src="https://raw.githubusercontent.com/pollinations/pollinations/main/assets/logo-text.svg" alt="pollinations.ai" width="400"/>
  
  <h3>Open-source AI for people who make things.</h3>
  
  <p>A community-driven platform where developers, artists, and tinkerers build together.<br/>No gatekeeping — just good tools and good people.</p>

[![Stars](https://img.shields.io/github/stars/pollinations/pollinations?style=flat-square&logo=github&label=Stars)](https://github.com/pollinations/pollinations)
[![License](https://img.shields.io/github/license/pollinations/pollinations?style=flat-square)](https://github.com/pollinations/pollinations/blob/main/LICENSE)
[![Discord](https://img.shields.io/discord/885844321461485618?style=flat-square&logo=discord&label=Discord&color=5865F2)](https://discord.gg/pollinations-ai-885844321461485618)
[![npm](https://img.shields.io/npm/v/@pollinations/react?style=flat-square&logo=npm&label=React%20Hooks)](https://www.npmjs.com/package/@pollinations/react)
![Readme Badge](https://img.shields.io/badge/pollinations.ai-ORIGINALS-8a2be2?style=flat-square&logo=data:image/svg+xml,%3Csvg%20xmlns%3D%22http://www.w3.org/2000svg%22%20viewBox%3D%220%200%20124%20124%22%3E%3Ccircle%20cx%3D%2262%22%20cy%3D%2262%22%20r%3D%2262%22%20fill%3D%22%23ffffff%22/%3E%3C/svg%3E&logoColor=white&labelColor=6a0dad)

[Website](https://pollinations.ai) · [Dashboard](https://enter.pollinations.ai) · [API Docs](https://github.com/pollinations/pollinations/blob/main/APIDOCS.md) · [Discord](https://discord.gg/pollinations-ai-885844321461485618)

</div>

---

## 🚀 Quick Start

> Get your API key at [enter.pollinations.ai](https://enter.pollinations.ai)

```bash
# Generate an image
curl 'https://gen.pollinations.ai/image/a%20cat?key=YOUR_API_KEY' -o image.jpg

# Generate text
curl 'https://gen.pollinations.ai/text/Hello?key=YOUR_API_KEY'

# OpenAI-compatible endpoint
curl 'https://gen.pollinations.ai/v1/chat/completions' \
  -H 'Authorization: Bearer YOUR_API_KEY' \
  -H 'Content-Type: application/json' \
  -d '{"model": "openai", "messages": [{"role": "user", "content": "Hello"}]}'
```

## ✨ What We Offer

| Feature                 | Description                                        |
| ----------------------- | -------------------------------------------------- |
| 🖼️ **Image Generation** | Flux, GPT Image, Seedream, Kontext, and more       |
| 🎬 **Video Generation** | Seedance, Veo — text-to-video (alpha)              |
| 💬 **Text Generation**  | GPT-5, Claude, Gemini, DeepSeek, Grok, Perplexity  |
| 🎵 **Audio**            | Text-to-speech with multiple voices                |
| 🌱 **Pollen Tiers**     | Earn daily credits by contributing — tiers in beta |
| 🤖 **MCP Server**       | AI assistants like Claude can generate directly    |
| 💯 **100% Open Source** | Code, roadmap, conversations — all public          |

## 📊 Community Stats

<!-- STATS:START -->

| Metric           | Count                                                                                                          |
| ---------------- | -------------------------------------------------------------------------------------------------------------- |
| ⭐ Stars         | ![Stars](https://img.shields.io/github/stars/pollinations/pollinations?style=flat-square&label=)               |
| 🍴 Forks         | ![Forks](https://img.shields.io/github/forks/pollinations/pollinations?style=flat-square&label=)               |
| 👥 Contributors  | ![Contributors](https://img.shields.io/github/contributors/pollinations/pollinations?style=flat-square&label=) |
| 🔄 Open PRs      | ![PRs](https://img.shields.io/github/issues-pr/pollinations/pollinations?style=flat-square&label=)             |
| 📦 npm Downloads | ![npm](https://img.shields.io/npm/dm/@pollinations/react?style=flat-square&label=)                             |

<!-- STATS:END -->

## 📦 Ecosystem

### Core Platform

- **[pollinations](https://github.com/pollinations/pollinations)** — Main repo: API backends, web frontend, React hooks, MCP server

### Integrations

- **[@pollinations/react](https://www.npmjs.com/package/@pollinations/react)** — React hooks for easy frontend integration
- **[@pollinations/model-context-protocol](https://www.npmjs.com/package/@pollinations/model-context-protocol)** — MCP server for AI assistants

## 🏗️ Architecture

```mermaid
flowchart TB
    A["🌸 gen.pollinations.ai<br/><i>Unified API Gateway</i>"]

      A --> I["🖼️ Image<br/>(<i>Flux, GPT Image, Seedream</i>)"]
      A --> V["🎬 Video<br/>(<i>Seedance, Veo</i>)"]
      A --> T["💬 Text<br/>(<i>GPT-5, Claude, Gemini, Grok</i>)"]
      A --> AU["🎵 Audio<br/>(<i>TTS, STT, Voices</i>)"]

      style A fill:#fce7f3,stroke:#be185d,color:#831843,stroke-width:2px
      style I fill:#dbeafe,stroke:#3b82f6,color:#1e3a8a
      style V fill:#fef3c7,stroke:#f59e0b,color:#92400e
      style T fill:#d1fae5,stroke:#10b981,color:#065f46
      style AU fill:#ede9fe,stroke:#8b5cf6,color:#5b21b6
      linkStyle default stroke:#94a3b8,stroke-width:3px
```

## 🤝 Get Involved

- 💬 **[Discord](https://discord.gg/pollinations-ai-885844321461485618)** — Chat with the community
- 🐛 **[Issues](https://github.com/pollinations/pollinations/issues)** — Report bugs or request features
- 📱 **[Submit Your App](https://github.com/pollinations/pollinations/issues/new?template=tier-app-submission.yml)** — Share what you've built

## 💚 Support Us

- ☕ **[Ko-fi](https://ko-fi.com/pollinationsai)** — One-time donations
- 💖 **[GitHub Sponsors](https://github.com/sponsors/pollinations)** — Monthly support
- 🌐 **[Open Collective](https://opencollective.com/pollinationsai)** — Transparent funding

## 📣 Stay Connected

<p align="center">
  <a href="https://twitter.com/pollinations_ai">𝕏 Twitter</a> · 
  <a href="https://instagram.com/pollinations_ai">Instagram</a> · 
  <a href="https://www.linkedin.com/company/pollinations-ai">LinkedIn</a> · 
  <a href="https://facebook.com/pollinations">Facebook</a> · 
  <a href="https://www.reddit.com/r/pollinations_ai/">Reddit</a> · 
  <a href="https://www.youtube.com/c/pollinations">YouTube</a>
</p>

## 🌍 Supported By

<p align="center">
  <a href="https://www.perplexity.ai/">Perplexity AI</a> · 
  <a href="https://aws.amazon.com/">AWS</a> · 
  <a href="https://io.net/">io.net</a> · 
  <a href="https://www.byteplus.com/">BytePlus</a> · 
  <a href="https://cloud.google.com/">Google Cloud</a> · 
  <a href="https://www.nvidia.com/en-us/deep-learning-ai/startups/">NVIDIA Inception</a> · 
  <a href="https://azure.microsoft.com/">Azure</a> · 
  <a href="https://www.cloudflare.com/">Cloudflare</a> · 
  <a href="https://www.scaleway.com/">Scaleway</a> · 
  <a href="https://modal.com/">Modal</a> · 
  <a href="https://api.navy/">NavyAI</a> · 
  <a href="https://nebius.com/">Nebius</a>
</p>

---

<div align="center">
  <sub>Made with ❤️ in Berlin · <a href="https://github.com/pollinations/pollinations/blob/main/LICENSE">MIT License</a></sub>
</div>
