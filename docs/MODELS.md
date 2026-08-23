# SokSam AI model system

SokSam AI presents a simple public tier system while using an adaptive backend routing layer.

## Public chat tiers

| Public tier | Intended use |
|---|---|
| **SokSam SuperFlash** | Fast, lightweight and instant answers |
| **SokSam Standard** | Reliable everyday conversations and work |
| **SokSam Nova** | Deeper tasks and more demanding workflows |
| **SokSam Max** | Highest-capability public workloads |

## Adaptive backend pool

The production platform currently works with **around 50 eligible underlying models** distributed behind these public tiers.

The backend model does not have to change on every request. A user may remain on the same eligible route for several messages when load is low and the route stays healthy. As concurrency grows, traffic can be distributed across other eligible models in the same tier.

The stable public contract is the SokSam tier name. Private provider identities, credentials, routing weights and fallback topology are intentionally not published.

For more detail, see [`ADAPTIVE-ROUTING.md`](ADAPTIVE-ROUTING.md).

## SokSam AI Studio models

SokSam AI Studio exposes a more granular eight-model lineup for API usage:

1. **SokSam SuperFlash**
2. **SokSam Standard Minimum**
3. **SokSam Standard Maximum**
4. **SokSam Nova Minimum**
5. **SokSam Nova Maximum**
6. **SokSam Max Minimum**
7. **SokSam Max Medium**
8. **SokSam Max Maximum / High**

Studio is currently available **only on computers / desktop browsers**.

Developers can create a SokSam API key in Studio and use the OpenAI-compatible integration information shown there with compatible software.

Studio: https://soksam.pp.ua/soksam/studio

## Development status

SokSam AI is in a deep-demo / rapid-development stage. The model pool, Studio lineup, limits and naming can evolve as the platform receives frequent updates.

For current product information, see https://soksam.pp.ua/models.
