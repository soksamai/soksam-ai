<div align="center">
  <a href="https://soksam.pp.ua/">
    <img src="https://soksam.pp.ua/soksam/brand/icon-512.png" width="104" alt="SokSam AI logo">
  </a>

# SokSam AI

**A multilingual AI workspace for chat, files, images, voice, projects and developer workflows.**

[![Official Website](https://img.shields.io/badge/Official_Website-soksam.pp.ua-111111?style=for-the-badge)](https://soksam.pp.ua/)
[![Open SokSam](https://img.shields.io/badge/Open-SokSam_AI-111111?style=for-the-badge)](https://soksam.pp.ua/soksam/chat)
[![Studio](https://img.shields.io/badge/SokSam_AI-Studio-111111?style=for-the-badge)](https://soksam.pp.ua/soksam/studio)
[![Telegram Channel](https://img.shields.io/badge/Telegram-News_Channel-111111?style=for-the-badge&logo=telegram)](https://t.me/vibescriptaibest)
[![Telegram Bot](https://img.shields.io/badge/Telegram-AI_Bot-111111?style=for-the-badge&logo=telegram)](https://t.me/vibescripthelper_bot)

<br>

<a href="https://soksam.pp.ua/">
  <img src="https://soksam.pp.ua/soksam/brand/social-card.png" alt="SokSam AI" width="100%">
</a>
</div>

---

## What is SokSam AI?

**SokSam AI** is an artificial intelligence workspace for conversations, supported files, image understanding, image generation, voice generation, organized project work and developer workflows.

This repository is the **official public GitHub repository for SokSam AI**. It contains product information, public architecture notes, documentation links, security guidance and issue reporting. The proprietary production application source code and private infrastructure are not published here.

> **Current status:** SokSam AI is in a **deep public demo / rapid-development stage**. The product is already usable, but it is still evolving quickly and is expected to receive substantial updates approximately every week. Interfaces, limits, model availability and pricing may change while the platform matures.

## At a glance

| Capability | What it provides |
|---|---|
| 🌍 **30 interface languages** | A multilingual product experience |
| 🧠 **~50-model adaptive backend pool** | Eligible models are selected dynamically according to tier, workload and availability |
| ⚡ **4 public chat tiers** | SuperFlash, Standard, Nova and Max |
| 📎 **File analysis** | Work with supported documents and files |
| 👁️ **Image understanding** | Analyze visual source material |
| 🎨 **Image generation** | Create images from written ideas |
| 🔊 **Voice generation** | Generate spoken audio from text in multiple languages, including Russian |
| 🗂️ **Projects & memory tools** | Projects, branches, bookmarks and explicit memory |
| 🌐 **Web + Telegram** | Use SokSam in the browser or as a conversational Telegram bot |
| 🧩 **SokSam AI Studio** | Desktop-only API workspace with OpenAI-compatible integration |

---

## Two ways to use SokSam AI

### 1. Web application

The main browser experience is available at:

**https://soksam.pp.ua/soksam/chat**

It provides the full SokSam workspace experience, including chat, files, images, projects, memory tools and other web features.

### 2. Telegram AI bot

For users who prefer Telegram instead of a browser, SokSam is also available as a conversational bot:

**[@vibescripthelper_bot](https://t.me/vibescripthelper_bot)**

The bot can be used as a normal Telegram conversation with the AI. Users can ask questions, interact with the assistant and also ask it about the associated Telegram channel and its content.

The primary Telegram news/community channel is:

**[VibeScript AI Best — @vibescriptaibest](https://t.me/vibescriptaibest)**

The channel publishes news and updates about neural networks, AI tools, SokSam AI and related technology topics.

See [`community/TELEGRAM.md`](community/TELEGRAM.md) and [`interfaces/ACCESS.md`](interfaces/ACCESS.md).

---

## Creator

SokSam AI is currently developed by **one primary developer, Viktor**.

The project uses a hybrid development workflow combining traditional software engineering with AI-assisted / vibe-coding techniques. As a rough description of the current workflow, development is approximately **50% direct human implementation and engineering by Viktor and 50% AI-assisted coding, refactoring, exploration and acceleration**.

This does not mean the AI independently owns or operates the project. Viktor defines the product direction, architecture, requirements, integration decisions, testing and final acceptance. AI systems are used as development tools to help create and refine code, including complex scripts and engineering tasks that go well beyond simple beginner examples.

Only the first name **Viktor** is being published at this stage. Additional creator information may be disclosed later.

Read more in [`project/CREATOR.md`](project/CREATOR.md) and [`project/DEVELOPMENT.md`](project/DEVELOPMENT.md).

---

## Adaptive model routing

SokSam AI does not expose one fixed backend model for every request. The production platform currently works with a pool of **around 50 eligible underlying models** distributed across the public SokSam tiers.

Routing is adaptive rather than random. The system can take into account the selected public tier, current traffic, model availability and workload distribution. A user can remain on the same eligible model for several consecutive requests — especially when traffic is low — while additional users and higher concurrency can cause the router to distribute work across other models in the same tier.

In practice this means that the backend model does **not** have to change on every message, but it can change dynamically as the service balances demand. The public contract remains stable: users choose a SokSam tier, while the internal routing layer decides which eligible backend model should serve the request.

Read more in [`docs/ADAPTIVE-ROUTING.md`](docs/ADAPTIVE-ROUTING.md).

## Public chat tiers

| Tier | Primary goal |
|---|---|
| **SokSam SuperFlash** | Very fast responses and lightweight tasks |
| **SokSam Standard** | Balanced everyday work |
| **SokSam Nova** | Deeper and more demanding tasks |
| **SokSam Max** | Highest-capability workloads |

The public tier names stay stable even when the private backend model selected inside a tier changes.

---

## SokSam AI Studio

**SokSam AI Studio** is the developer workspace for using SokSam through API keys and OpenAI-compatible integrations.

➡️ **Studio:** https://soksam.pp.ua/soksam/studio

> **Desktop availability:** SokSam AI Studio is currently available **only on computers / desktop browsers**. The regular SokSam chat remains available separately on supported devices.

Studio currently provides:

- creation and management of personal SokSam API keys;
- an **OpenAI-compatible** integration flow and base URL information inside Studio;
- the ability to connect SokSam API keys to applications and tools that support compatible API endpoints;
- usage and balance information;
- a **$5 starting test balance** for new Studio usage;
- eight Studio model choices spanning speed, balance and maximum-capability workloads.

### Studio model lineup

1. **SokSam SuperFlash**
2. **SokSam Standard Minimum**
3. **SokSam Standard Maximum**
4. **SokSam Nova Minimum**
5. **SokSam Nova Maximum**
6. **SokSam Max Minimum**
7. **SokSam Max Medium**
8. **SokSam Max Maximum / High**

At the moment, **Free is the only available subscription tier**. Paid subscriptions are not implemented yet. The Studio model catalog, limits, pricing and naming may evolve during the deep-demo period.

Full public notes: [`docs/STUDIO.md`](docs/STUDIO.md).

---

## Voice generation

SokSam AI now includes a text-to-speech / voice-generation workflow.

Enable the voice-generation function, enter text of up to **500 characters**, choose or use the available language/voice option, and SokSam returns generated spoken audio. Voice generation supports multiple languages, including **Russian**.

This feature is part of the actively evolving demo and may gain additional voices, languages and controls over time.

See [`docs/VOICE.md`](docs/VOICE.md).

---

## How the public product fits together

```mermaid
flowchart LR
    U[User] --> C[SokSam Web Chat]
    U --> TB[Telegram Bot]
    U --> S[SokSam AI Studio - Desktop]
    TB --> R[Adaptive Router]
    C --> R
    R --> SF[SuperFlash pool]
    R --> ST[Standard pool]
    R --> NV[Nova pool]
    R --> MX[Max pool]
    C --> F[Files / Images / Voice]
    S --> K[Personal API Key]
    K --> O[OpenAI-compatible integrations]
    CH[Telegram News Channel] --> U
```

This diagram is intentionally conceptual. Private provider identities, credentials, routing weights and infrastructure topology are not published.

---

## Repository structure

| Area | Purpose |
|---|---|
| [`docs/`](docs/) | Technical and product documentation |
| [`project/`](project/) | Creator, ownership and development workflow |
| [`community/`](community/) | Official community and Telegram presence |
| [`interfaces/`](interfaces/) | Ways to access SokSam AI |
| [`roadmap/`](roadmap/) | Public direction and demo-stage roadmap |
| [`.github/`](.github/) | GitHub issue and repository configuration |

## Documentation in this repository

| Document | Purpose |
|---|---|
| [`project/CREATOR.md`](project/CREATOR.md) | Public creator information |
| [`project/DEVELOPMENT.md`](project/DEVELOPMENT.md) | Human + AI-assisted development model |
| [`community/TELEGRAM.md`](community/TELEGRAM.md) | Official Telegram channel and bot |
| [`interfaces/ACCESS.md`](interfaces/ACCESS.md) | Web, Telegram and Studio access |
| [`roadmap/README.md`](roadmap/README.md) | Public deep-demo roadmap |
| [`docs/CURRENT-STATUS.md`](docs/CURRENT-STATUS.md) | Current deep-demo status and update cadence |
| [`docs/ADAPTIVE-ROUTING.md`](docs/ADAPTIVE-ROUTING.md) | How the ~50-model adaptive pool behaves publicly |
| [`docs/MODELS.md`](docs/MODELS.md) | Public tiers and Studio model lineup |
| [`docs/STUDIO.md`](docs/STUDIO.md) | Studio, API keys, starting balance and desktop availability |
| [`docs/VOICE.md`](docs/VOICE.md) | Voice generation and current 500-character limit |
| [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md) | High-level public architecture |
| [`docs/BRAND.md`](docs/BRAND.md) | Official SokSam AI identity |
| [`docs/OFFICIAL-LINKS.md`](docs/OFFICIAL-LINKS.md) | First-party links |
| [`SECURITY.md`](SECURITY.md) | Security and reporting guidance |

---

## Explore SokSam AI

- 🌐 [Official website](https://soksam.pp.ua/)
- 💬 [Open SokSam AI](https://soksam.pp.ua/soksam/chat)
- 🧩 [SokSam AI Studio — desktop only](https://soksam.pp.ua/soksam/studio)
- 📰 [Telegram news channel](https://t.me/vibescriptaibest)
- 🤖 [Telegram AI bot](https://t.me/vibescripthelper_bot)
- ✨ [Features](https://soksam.pp.ua/features)
- 🧠 [Model tiers](https://soksam.pp.ua/models)
- 📚 [Documentation](https://soksam.pp.ua/docs)
- 📰 [Changelog](https://soksam.pp.ua/changelog)
- 🔐 [Security](https://soksam.pp.ua/security)
- 🛡️ [Privacy](https://soksam.pp.ua/privacy)
- 📡 [RSS feed](https://soksam.pp.ua/feed.xml)

More first-party links are collected in [`docs/OFFICIAL-LINKS.md`](docs/OFFICIAL-LINKS.md).

## Privacy and security

Private chats, account pages, administration routes and Studio data are deliberately kept outside the public website sitemap and search indexing.

Never post passwords, API keys, tokens, private conversations, personal data, infrastructure secrets or security vulnerabilities in a public GitHub issue.

See [`SECURITY.md`](SECURITY.md) for reporting guidance.

## Issues and feedback

GitHub Issues are intended for reproducible public product bugs, documentation corrections, broken public links, accessibility feedback and clear public feature feedback.

Do not use public issues for credentials, account-specific private information, private conversation content or vulnerability details.

---

<div align="center">
  <strong>SokSam AI</strong><br>
  Chat · Explore · Create · Build
  <br><br>
  <a href="https://soksam.pp.ua/">Website</a> ·
  <a href="https://soksam.pp.ua/soksam/studio">Studio</a> ·
  <a href="https://t.me/vibescriptaibest">Telegram Channel</a> ·
  <a href="https://t.me/vibescripthelper_bot">Telegram Bot</a> ·
  <a href="https://soksam.pp.ua/docs">Docs</a>
  <br><br>
  © 2026 SokSam AI. All rights reserved.
</div>
