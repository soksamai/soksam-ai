# SokSam AI — Public Product Overview

SokSam AI is a multilingual artificial intelligence workspace that combines conversational AI, file and image work, voice generation, project organization and developer access in one product family.

This document intentionally describes the product from a public, user-facing perspective. Private provider identities, credentials, internal routing rules, administrative mechanisms and production infrastructure are not part of this document.

## Product status

SokSam AI is currently in a **deep public demo / rapid-development stage**. The product is already usable, but development is active and substantial updates are expected regularly, approximately every week.

During this stage, interfaces, limits, model availability, pricing and individual experimental capabilities may change.

## Main ways to use SokSam AI

### Web application

The primary browser application is available at:

https://soksam.pp.ua/soksam/chat

The web experience brings together chat, model selection, files, images, voice tools, projects, bookmarks, memory-related features and account settings.

### Telegram AI bot

Users who prefer Telegram can interact with the AI directly through:

https://t.me/vibescripthelper_bot

The Telegram bot provides a conversational alternative to the browser experience and can also help users learn about the associated Telegram channel.

### SokSam AI Studio

Developer access is available through:

https://soksam.pp.ua/soksam/studio

Studio is currently **desktop-only** and is designed for creating and managing SokSam API keys and connecting compatible applications through an OpenAI-compatible workflow.

## Core capabilities

### Conversational AI

SokSam AI provides streaming conversations with four stable public tiers:

- **SokSam SuperFlash** — focused on speed and lightweight tasks
- **SokSam Standard** — balanced everyday work
- **SokSam Nova** — deeper and more demanding tasks
- **SokSam Max** — the highest-capability public tier

The public tier names remain stable while SokSam can dynamically select an eligible internal model from its adaptive pool.

### Adaptive model pool

The current production platform works with a pool of **around 50 eligible models** distributed across the public SokSam tiers.

The internal selection can change according to factors such as the chosen tier, availability and workload. A user may stay on the same eligible model for several consecutive requests, while higher concurrency can cause work to be distributed differently.

This is intentionally a public conceptual description. Exact routing rules, weights, fallback order and internal provider details are private.

### Files and documents

SokSam can work with supported documents, spreadsheets, text files, images, archives and email files. Depending on the file type, the application can extract useful content and make it available to the conversation for analysis.

Current public file documentation is available in [`FILE-SUPPORT.md`](FILE-SUPPORT.md).

### Image understanding

Users can attach images and ask questions about visual content, screenshots, diagrams, charts and other supported images.

### Image generation

SokSam includes image-generation workflows integrated with the conversational experience. Generated images can be returned as conversation artifacts.

### Voice generation

SokSam includes text-to-speech generation in multiple languages, including Russian. The current public text limit is **500 characters per generation**.

See [`VOICE.md`](VOICE.md).

### Projects and organization

SokSam includes tools for organizing longer work:

- projects for grouping related conversations;
- conversation branches for exploring alternative directions;
- bookmarks for saving important messages;
- explicit memory-related tools for persistent user context.

These capabilities are designed to make SokSam useful for work that continues beyond a single chat session.

## SokSam AI Studio

Studio is the developer-oriented part of SokSam AI.

Current public capabilities include:

- creation and management of personal API keys;
- OpenAI-compatible integration guidance;
- usage and balance information;
- multiple SokSam model variants;
- a **$5 starting test balance**;
- connection to compatible third-party applications and developer tools.

Current Studio models:

1. SokSam SuperFlash
2. SokSam Standard Minimum
3. SokSam Standard Maximum
4. SokSam Nova Minimum
5. SokSam Nova Maximum
6. SokSam Max Minimum
7. SokSam Max Medium
8. SokSam Max Maximum / High

The only currently implemented subscription tier is **Free**. Paid subscriptions are not yet available.

See [`STUDIO.md`](STUDIO.md).

## Multilingual interface

The SokSam web interface currently supports **30 UI languages**, covering major European languages as well as Arabic, Chinese, Japanese and Korean.

See [`LANGUAGES.md`](LANGUAGES.md) for the public language list.

## Telegram news and community

The primary Telegram news/community channel is:

https://t.me/vibescriptaibest

It publishes news and updates about neural networks, AI tools, SokSam AI and related technology topics.

See [`../community/TELEGRAM.md`](../community/TELEGRAM.md).

## Development model

SokSam AI is currently developed primarily by **Viktor**, the founder, owner and primary developer of the project.

Development combines direct software engineering with AI-assisted / vibe-coding workflows. The current development balance is publicly described approximately as **50% direct human development and 50% AI-assisted development**. This is a workflow description, not a strict measurement of lines of code.

See [`../project/CREATOR.md`](../project/CREATOR.md) and [`../project/DEVELOPMENT.md`](../project/DEVELOPMENT.md).

## Public links

- Website: https://soksam.pp.ua/
- Web app: https://soksam.pp.ua/soksam/chat
- Studio: https://soksam.pp.ua/soksam/studio
- Telegram channel: https://t.me/vibescriptaibest
- Telegram bot: https://t.me/vibescripthelper_bot
- GitHub: https://github.com/soksamai/soksam-ai

## Publication boundary

The public SokSam documentation deliberately does **not** publish credentials, private model-provider identities, private model IDs, internal routing logic, internal service endpoints, production filesystem paths, administrative security details or infrastructure topology.
