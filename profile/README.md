<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/pollinations/pollinations/main/packages/ui/src/brand/lockup-stacked-white.svg" />
    <img src="https://raw.githubusercontent.com/pollinations/pollinations/main/packages/ui/src/brand/lockup-stacked-black.svg" alt="Pollinations.ai" width="128" />
  </picture>

  <p>Artists and developers build open-source AI tools here. Explore a community app, try a model, or share something of your own.</p>

[![Stars](https://img.shields.io/github/stars/pollinations/pollinations?style=flat-square&logo=github&label=Stars)](https://github.com/pollinations/pollinations)
[![License](https://img.shields.io/github/license/pollinations/pollinations?style=flat-square)](https://github.com/pollinations/pollinations/blob/main/LICENSE)
[![Discord](https://img.shields.io/discord/885844321461485618?style=flat-square&logo=discord&label=Discord&color=5865F2)](https://discord.gg/k9F7SyTgqn)
[![npm](https://img.shields.io/npm/v/@pollinations/sdk?style=flat-square&logo=npm&label=Pollinations%20SDK)](https://www.npmjs.com/package/@pollinations/sdk)
![Readme Badge](https://img.shields.io/badge/pollinations.ai-ORIGINALS-8a2be2?style=flat-square&logo=data:image/svg+xml,%3Csvg%20xmlns%3D%22http://www.w3.org/2000svg%22%20viewBox%3D%220%200%20124%20124%22%3E%3Ccircle%20cx%3D%2262%22%20cy%3D%2262%22%20r%3D%2262%22%20fill%3D%22%23ffffff%22/%3E%3C/svg%3E&logoColor=white&labelColor=6a0dad)

[Ecosystem](#ecosystem) · [Get involved](#get-involved) · [Playground](https://pollinations.ai/play) · [Community apps](https://pollinations.ai/apps) · [Main repository](https://github.com/pollinations/pollinations)

</div>

<p align="center"><img src="https://media.pollinations.ai/0c5d756a-6beb-4cdb-88b0-e9f4885e355f" alt="Under a lime awning, Polli offers seeds to Monitor Robot, who holds an empty flowerpot." width="800" /></p>

---

## Ecosystem

| Explore | What you can do |
| --- | --- |
| [Models](https://enter.pollinations.ai/models) | Chat, edit a photo, animate a still, or make music. The same API supports transcription, 3D assets, and embeddings for search. |
| [Community models](https://enter.pollinations.ai/models?q=source%3Acommunity) | Try a model hosted by another builder or connect your own endpoint to the catalog. |
| [Community agents](https://enter.pollinations.ai/agents) and [MCP tools](https://gen.pollinations.ai/docs#tag/mcp-servers) | Give an agent instructions and tools to search the web or work with connected apps. Share it so others can call it by name. |
| [Sandboxes](https://gen.pollinations.ai/docs#tag/sandboxes) | Open a Linux machine in VS Code or over SSH. Run a project, test a change, and preview it with your agent. |
| [Sites](https://gen.pollinations.ai/docs#tag/sites) and [media storage](https://github.com/pollinations/pollinations/blob/main/APIDOCS.md#media-storage) | Publish a static site at `your-name.pollinations.app` or upload media to use in your next model call. |
| [Pollinations Pay](https://gen.pollinations.ai/docs#tag/pollinations-pay) | Let people sign in to your app, set a spending limit, and pay from their own balance. |

## Get involved

- **Share an app.** [Submit it to the gallery](https://github.com/pollinations/pollinations/issues/new?template=app-submission.yml) so others can try it.
- **Publish a model or agent.** [Request publisher access](https://github.com/pollinations/pollinations/issues/new?template=community-model-allowlist.yml), then follow the guide for [models](https://gen.pollinations.ai/docs#tag/publish-a-model) or [agents](https://gen.pollinations.ai/docs#tag/publish-an-agent).
- **Solve an issue.** Pick an [open issue](https://github.com/pollinations/pollinations/issues), test your change, and link it in your pull request. For example, [PR #19797](https://github.com/pollinations/pollinations/pull/19797) fixed [#19792](https://github.com/pollinations/pollinations/issues/19792) so the playground keeps your prompt and settings after sign-in. [Contributor guide](https://github.com/pollinations/pollinations/blob/main/CONTRIBUTING.md)
- **Meet other builders.** Share a project in **#showcase** or ask for help in **#code-help**. [Join Discord](https://discord.gg/k9F7SyTgqn)

### Earnings and Quests

Model publishers earn a share when people use a priced model. App developers can enable earnings on paid requests. [Model pricing](https://gen.pollinations.ai/docs#tag/publish-a-model) · [App earnings](https://gen.pollinations.ai/docs#tag/pollinations-pay)

Each Quest lists a task and its reward. For a coding Quest, link your pull request to the issue. Once maintainers select and merge your fix, claim the reward in the [Quests dashboard](https://enter.pollinations.ai/quests).

## Developer tools

Try a prompt in the [playground](https://pollinations.ai/play), use the [CLI](https://github.com/pollinations/pollinations/tree/main/packages/polli-cli) from your terminal, or add the [SDK](https://github.com/pollinations/pollinations/tree/main/packages/sdk) to a JavaScript, TypeScript, or React app. For a first API call and more examples, see the [API quick start](https://github.com/pollinations/pollinations/blob/main/APIDOCS.md#-getting-started) and [API reference](https://gen.pollinations.ai/docs).

## 📊 Community Stats

<!-- STATS:START -->

| Metric           | Count                                                                                                          |
| ---------------- | -------------------------------------------------------------------------------------------------------------- |
| ⭐ Stars         | ![Stars](https://img.shields.io/github/stars/pollinations/pollinations?style=flat-square&label=)               |
| 🍴 Forks         | ![Forks](https://img.shields.io/github/forks/pollinations/pollinations?style=flat-square&label=)               |
| 👥 Contributors  | ![Contributors](https://img.shields.io/github/contributors/pollinations/pollinations?style=flat-square&label=) |
| 🔄 Open PRs      | ![PRs](https://img.shields.io/github/issues-pr/pollinations/pollinations?style=flat-square&label=)             |
| 📦 SDK downloads | ![npm](https://img.shields.io/npm/dm/@pollinations/sdk?style=flat-square&label=)                             |

<!-- STATS:END -->

## 🏗️ Platform at a glance

```mermaid
flowchart TB
    A["🌸 Pollinations.ai"]

      A --> I["🎨 Models"]
      A --> V["🤖 Agents and tools"]
      A --> T["💻 Sandboxes"]
      A --> AU["🌐 Sites and media"]

      style A fill:#fce7f3,stroke:#be185d,color:#831843,stroke-width:2px
      style I fill:#dbeafe,stroke:#3b82f6,color:#1e3a8a
      style V fill:#fef3c7,stroke:#f59e0b,color:#92400e
      style T fill:#d1fae5,stroke:#10b981,color:#065f46
      style AU fill:#ede9fe,stroke:#8b5cf6,color:#5b21b6
      linkStyle default stroke:#94a3b8,stroke-width:3px
```

## 📣 Stay Connected

<p align="center">
  <a href="https://x.com/pollinations_ai">𝕏</a> ·
  <a href="https://instagram.com/pollinations_ai">Instagram</a> ·
  <a href="https://www.linkedin.com/company/pollinations-ai">LinkedIn</a> ·
  <a href="https://facebook.com/pollinations">Facebook</a> ·
  <a href="https://www.reddit.com/r/pollinations_ai/">Reddit</a> ·
  <a href="https://www.youtube.com/c/pollinations">YouTube</a>
</p>

## 🌍 Supported By

<!-- website-supporters:start -->
[Alibaba Cloud](https://www.alibabacloud.com/) · [Anthropic](https://www.anthropic.com/) · [AssemblyAI](https://www.assemblyai.com/) · [AWS](https://aws.amazon.com/) · [BytePlus](https://www.byteplus.com/) · [Cloudflare](https://developers.cloudflare.com/workers-ai/) · [Daytona](https://www.daytona.io/) · [DigitalOcean](https://www.digitalocean.com/) · [E2B](https://e2b.dev/) · [ElevenLabs](https://elevenlabs.io/) · [Exa](https://exa.ai/) · [Fireworks AI](https://fireworks.ai/) · [Google Cloud](https://cloud.google.com/) · [InferencePort AI](https://inferenceport.ai/) · [io.net](https://io.net/) · [Lambda](https://lambda.ai/) · [Microsoft Azure](https://azure.microsoft.com/) · [Modal](https://modal.com/) · [Nebius](https://nebius.com/) · [NVIDIA](https://www.nvidia.com/en-us/deep-learning-ai/startups/) · [OpenAI](https://openai.com/) · [OpenRouter](https://openrouter.ai/) · [OVHcloud](https://www.ovhcloud.com/) · [Perplexity](https://www.perplexity.ai/) · [RunPod](https://www.runpod.io/) · [Scaleway](https://www.scaleway.com/)
<!-- website-supporters:end -->


---

<div align="center">
  <sub>Made with ❤️ in Berlin · <a href="https://github.com/pollinations/pollinations/blob/main/LICENSE">MIT License</a></sub>
</div>
