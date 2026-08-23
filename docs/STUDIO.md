# SokSam AI Studio

**SokSam AI Studio** is the developer-facing workspace for creating SokSam API keys and connecting SokSam models to external applications through an OpenAI-compatible integration flow.

Official Studio URL: https://soksam.pp.ua/soksam/studio

> **Availability:** Studio is currently available **only on computers / desktop browsers**. It is not currently presented as a full mobile Studio experience.

## What Studio provides

Studio currently includes:

- creation and management of personal SokSam API keys;
- OpenAI-compatible connection information;
- the base URL and integration details needed by compatible clients;
- model selection;
- balance and usage information;
- a **$5 starting balance** intended for initial testing and experimentation.

An API key created in Studio can be used with software that supports the compatible API format, subject to the current SokSam limits and model availability.

## Current Studio model lineup

Studio currently exposes eight model choices:

| Studio model | Positioning |
|---|---|
| **SokSam SuperFlash** | Fastest Studio route |
| **SokSam Standard Minimum** | Lighter Standard route |
| **SokSam Standard Maximum** | Stronger Standard route |
| **SokSam Nova Minimum** | Lighter Nova route |
| **SokSam Nova Maximum** | Stronger Nova route |
| **SokSam Max Minimum** | Entry Max route |
| **SokSam Max Medium** | Mid-level Max route |
| **SokSam Max Maximum / High** | Highest Studio Max route |

The Studio lineup is distinct from the simpler four-tier chat interface. It gives developers more control over the capability level they want to call through an API key.

## OpenAI-compatible workflow

Studio is designed so compatible developer tools can be configured with:

1. a SokSam API key;
2. the OpenAI-compatible base URL shown in Studio;
3. one of the supported SokSam Studio model choices.

The exact endpoint details and current model identifiers should always be taken from the live Studio interface because they can evolve during the demo period.

## Subscription status

At this time, **Free is the only implemented subscription tier**. Paid subscription plans are not yet available.

The $5 starting balance is intended to make testing possible before future subscription and billing options are introduced.

## Development status

Studio is part of the current **deep-demo / rapid-development** version of SokSam AI. It is already usable, but model names, limits, balance rules, pricing and integration details may change as the platform is updated.

Never publish SokSam API keys in GitHub issues, repositories, screenshots, browser URLs or public logs.
