# SokSam AI — Public feature guide

SokSam AI combines conversational work, research, creation, multi-file projects, personal files and developer access. This guide focuses on user-facing features rather than private providers or infrastructure.

## Choose your workflow

| Workspace | Purpose | Access |
|---|---|---|
| **Chat** | Ask, research, analyze files and create downloadable materials | [Web app](https://soksam.pp.ua/soksam/chat) |
| **Agent** | Create or revise websites, games, bots, applications and tools spanning multiple files | **Agent** in the signed-in web app's left menu |
| **My Files** | Organize source files, generated work and Agent project folders | Signed-in web app |
| **Studio** | API keys, compatible integrations, usage and shared virtual credits | [Desktop Studio](https://soksam.pp.ua/soksam/studio) |
| **Telegram bot** | An alternative conversational interface and its supported bot features | [@vibescripthelper_bot](https://t.me/vibescripthelper_bot) |

## Capabilities by interface

| Capability | Browser workspace | Telegram | Studio |
|---|---|---|---|
| AI conversation | Yes | Yes | Through API |
| Four public Chat levels | Yes | Supported model modes | Eight Studio variants, not the same list |
| Search with sources and deeper research | Chat | Not promised here | Not promised here |
| Read supported attachments | Chat | Supported bot workflows | Depends on API compatibility |
| Create Word/PDF, Excel/CSV, charts and PowerPoint | Chat workflows | Not promised here | Not promised here |
| Understand or generate images | Chat | Image understanding in supported bot flows | Depends on supported API |
| Browser voice input / generated speech | Supported browser voice tools / text-to-speech | Bot-dependent | Not promised here |
| Conversation projects, branches, bookmarks and explicit memory | Chat | Bot-specific memory features | — |
| Build multi-file projects with progress and supported previews | **Agent** | Separate bot coding mode | — |
| File folders, viewers, editing, trash and versions | **My Files** | — | Shared balance funds extra storage |
| API keys, model IDs and credit history | — | — | Yes |

An entry marked “not promised here” does not claim a feature is impossible; it avoids assuming every interface exposes the same workflow.

## Chat, models and research

The public chat levels are **SuperFlash**, **Standard**, **Nova** and **Max**. The interface supports **30 languages**, and the platform uses an adaptive pool of **around 50 eligible underlying models**; the specific model can vary by workload and availability.

Chat supports web search with sources, deeper comparisons, document and data workflows, image understanding and generation, and longer work through projects and memory tools. Browser voice input depends on browser support; text-to-speech is available in supported languages, including Russian, with a previously documented 500-character text limit per generation.

[Search & research](SEARCH-AND-RESEARCH.md) · [Create & export](CREATE-AND-EXPORT.md) · [Models](MODELS.md) · [Voice](VOICE.md)

## Agent projects

Agent is **available to signed-in users**, not a future-only roadmap item or owner-only tool. It can plan, edit multiple files, run available checks, show progress and save versions. Projects have dedicated folders and conversations; supported websites and games can be previewed. Execution happens in a server-side isolated environment.

[Agent guide](AGENT.md)

## My Files

My Files stores sources and outputs, with folders, search, recent items, move/copy/download, supported viewers and editing, versions, trash recovery and ZIP operations within limits. The base storage is **2 GB**; extra space uses the shared Studio virtual credit balance. Antivirus-check status is visible without promising absolute safety.

[My Files](MY-FILES.md) · [Attachment limits](FILE-SUPPORT.md)

## Developer Studio and credits

Desktop Studio provides personal API keys, OpenAI-compatible connection information, eight Studio model choices, usage reporting and credit history. One virtual credit balance (displayed in USD but not withdrawable) is shared across **Agent, API requests and extra My Files storage**. Ordinary Chat does not consume these credits, though other usage limits apply.

There is an initial **$5** account credit, **$1** claimed by opening Studio once per UTC day, and a conditional **one-time $10 Telegram bonus**. See the exact verification steps in [CREDITS.md](CREDITS.md). **Free** remains the only available subscription plan; purchases and paid plans are not implemented.

[Studio](STUDIO.md) · [Credits](CREDITS.md)

## Demo status

SokSam AI is an actively developed deep public demo. Availability, limits and terms can change. For dated updates, see the [official changelog](https://soksam.pp.ua/changelog).
