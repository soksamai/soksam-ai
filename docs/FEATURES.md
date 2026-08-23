# SokSam AI — Public Feature Guide

This page summarizes the user-facing capabilities currently documented for SokSam AI. It intentionally excludes private infrastructure, provider identities, internal administrative systems and proprietary routing details.

## Feature matrix

| Feature | Web app | Telegram bot | Studio | Notes |
|---|---:|---:|---:|---|
| Conversational AI | Yes | Yes | API | Four public SokSam tiers |
| Streaming responses | Yes | Yes | Yes | Real-time response delivery where supported |
| Model selection | Yes | Yes | Yes | Public tier/model choices vary by interface |
| File analysis | Yes | Supported workflows | API-compatible workflows | Supported formats depend on interface |
| Image understanding | Yes | Yes | Compatible workflows | Analyze supported images and screenshots |
| Image generation | Yes | Interface-dependent | Compatible workflows | Returned as generated artifacts |
| Voice generation | Yes | Interface-dependent | — | Up to 500 characters per generation in the current demo |
| Voice input | Browser-dependent | — | — | Uses supported browser capabilities |
| Projects | Yes | — | — | Organize related conversations |
| Branches | Yes | — | — | Explore alternate conversation paths |
| Bookmarks | Yes | — | — | Save important messages |
| Memory tools | Yes | Yes in supported bot workflows | — | Persistent context features |
| 30-language UI | Yes | Language support available | Documentation/interface-dependent | Full web UI language set documented separately |
| API keys | — | — | Yes | Managed through SokSam AI Studio |
| OpenAI-compatible integration | — | — | Yes | For compatible developer tools and applications |
| Usage/balance view | — | — | Yes | Studio account information |
| Telegram news/community | Link from product | Yes | — | Main channel: @vibescriptaibest |

## Chat

The chat experience is the center of SokSam AI. Users can start conversations, choose a public model tier, receive streaming answers and continue work across multiple sessions.

Public tiers:

- **SokSam SuperFlash**
- **SokSam Standard**
- **SokSam Nova**
- **SokSam Max**

## Files

Supported public workflows include common documents, spreadsheets, text files, images, archives and email files. See [`FILE-SUPPORT.md`](FILE-SUPPORT.md) for current details and limits.

## Images

SokSam supports both understanding and generation workflows. Users can attach supported visual material for analysis, or request newly generated images from the conversational interface.

## Voice

Voice-generation support converts text to spoken audio in multiple languages, including Russian. The current public limit is 500 characters per generation.

## Projects and organization

Projects, branches and bookmarks allow users to organize work that spans more than one message or one conversation. These features are part of SokSam's goal of functioning as an AI workspace rather than only a single-turn chatbot.

## Developer Studio

SokSam AI Studio provides personal API keys, OpenAI-compatible integration, usage information and eight public Studio model variants. Studio is currently available only on desktop/computer browsers.

See [`STUDIO.md`](STUDIO.md).

## Telegram

The Telegram AI bot is available at:

https://t.me/vibescripthelper_bot

The public news/community channel is:

https://t.me/vibescriptaibest

The channel focuses on AI, neural networks, tools, SokSam updates and related technology news.

## Demo-stage notice

SokSam AI is in a deep public demo / rapid-development stage. Individual capabilities, limits and interface behavior may evolve as the project is updated.
