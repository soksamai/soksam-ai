# SokSam AI — Public Technical Scope

SokSam AI is more than a single chat interface. From a public engineering perspective, the project combines multiple product surfaces and several categories of functionality that have to work together consistently.

This page deliberately stays at a high level. It does not publish private infrastructure, provider identities, credentials, internal service endpoints, administrative mechanisms or security-sensitive routing details.

## Multi-interface product

SokSam AI currently spans:

- a browser-based AI workspace;
- a Telegram AI experience;
- a desktop-only developer Studio;
- a public website and documentation surface.

Keeping these interfaces consistent requires shared product concepts such as accounts, model tiers, usage rules, supported capabilities and public documentation.

## Real-time conversational experience

The chat experience supports streaming responses rather than waiting for an entire answer to finish before displaying it. This affects UI state, cancellation, error handling, message persistence and the way long-running generations are represented to users.

## Adaptive model abstraction

SokSam exposes stable public model tiers while internally working with a much larger eligible model pool. The engineering challenge is to preserve a consistent product contract even while availability and workload can change over time.

The current public tiers are:

- SokSam SuperFlash
- SokSam Standard
- SokSam Nova
- SokSam Max

The current platform uses a pool of around 50 eligible models, but exact provider identities and routing logic are private.

## Multimodal workflows

The product combines several different input and output types:

- text conversations;
- document and spreadsheet analysis;
- image understanding;
- image generation;
- voice generation;
- browser-supported voice input;
- generated downloadable artifacts.

Each workflow has different validation, user-interface and error-handling requirements.

## Long-running work

Projects, conversation branches, bookmarks and memory-related tools extend SokSam beyond single-session chat. They introduce persistent organization and navigation requirements that have to remain understandable across repeated use.

## Developer platform

SokSam AI Studio adds a second product layer for developers. It includes API-key management, model selection, usage information and an OpenAI-compatible integration workflow.

Studio is currently available only on desktop/computer browsers.

## Internationalization

The web interface supports 30 UI languages. Maintaining a multilingual application affects navigation, settings, authentication screens, notifications, documentation and layout behavior, including right-to-left presentation where appropriate.

See [`../docs/LANGUAGES.md`](../docs/LANGUAGES.md).

## Quality and reliability

The project includes automated testing across major functional areas and is updated frequently. Public documentation avoids exposing internal test topology or security implementation details, but testing is part of the regular development process.

See [`QUALITY.md`](QUALITY.md).

## Development model

SokSam AI is currently developed primarily by Viktor using a hybrid workflow that combines direct engineering with AI-assisted development. Product direction, architecture, integration, testing and final acceptance remain human-controlled.

See [`CREATOR.md`](CREATOR.md) and [`DEVELOPMENT.md`](DEVELOPMENT.md).

## Public boundary

The following intentionally remain private:

- credentials and secrets;
- real internal model/provider identities;
- exact routing rules and fallback order;
- administrative endpoints and controls;
- production network or filesystem topology;
- internal security thresholds and implementation details.

The goal of this repository is to explain SokSam AI as a product without publishing information that would unnecessarily expose its private production implementation.
