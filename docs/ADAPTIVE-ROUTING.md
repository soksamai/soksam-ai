# SokSam AI adaptive model routing

SokSam AI uses an adaptive routing layer instead of permanently attaching every public tier to one fixed backend model.

## Current model pool

The production service currently works with a pool of **around 50 eligible underlying models**. These models are grouped behind the stable public SokSam tiers:

- **SokSam SuperFlash** — fastest and lightweight routes;
- **SokSam Standard** — balanced everyday routes;
- **SokSam Nova** — deeper and more demanding routes;
- **SokSam Max** — highest-capability routes.

The exact private provider identities, credentials, weights and fallback topology are not part of the public contract.

## How selection behaves

Routing is dynamic, but that does not mean a completely different model must be selected on every message.

A user may stay on the same eligible model for several consecutive requests. This can happen when traffic is low, the current model remains healthy and there is no reason to move the workload.

As more users become active, the router can distribute traffic across other eligible models in the same public tier. The same principle applies when availability or workload changes.

A simplified public view is:

```text
Public tier
    ↓
Adaptive routing layer
    ↓
Eligible model pool for that tier
    ↓
Selected healthy route
```

## Why SokSam uses this design

The goal is to keep the user-facing product simple while allowing the backend to adapt to real demand.

The routing layer is designed to support:

- workload distribution when multiple users are active;
- continued service when one eligible route is unavailable;
- matching faster models to speed-oriented tiers;
- reserving stronger model classes for higher-capability tiers;
- changing internal routing without forcing users to learn private provider names.

## What stays stable for users

Users choose a SokSam tier rather than a private provider model. The public names — SuperFlash, Standard, Nova and Max — are intended to remain the stable interface even while the underlying routing pool evolves.

Because SokSam AI is currently in a deep-demo / rapid-development stage, the size and composition of the internal pool can change over time.
