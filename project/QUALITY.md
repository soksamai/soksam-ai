# SokSam AI — Quality and Reliability

SokSam AI is developed as a rapidly evolving public demo, but the project still uses structured testing and validation to reduce regressions as new features are introduced.

This document describes quality practices only at a public level. It intentionally avoids internal security tests, private infrastructure checks, provider-specific tests and operational details.

## Areas covered by automated testing

The project contains automated tests across major areas such as:

- core SokSam application behavior;
- conversational generation flows;
- file and attachment handling;
- authentication and authorization behavior;
- developer Studio/API behavior;
- model availability and routing behavior at an abstract level;
- Telegram workflows;
- user data operations;
- rate-limit behavior;
- project and agent-related workflows;
- persistence and data integrity.

## Unit and integration testing

The codebase includes both focused unit tests and broader integration-style tests. This allows individual functions to be checked in isolation while also validating that larger product flows still work together.

## Async behavior

Because several product workflows involve asynchronous operations and streaming, the test suite also includes coverage for asynchronous behavior rather than treating the application as purely synchronous.

## Release validation

New versions are expected to go through functional validation before being treated as production-ready. This is particularly important because SokSam AI is updated frequently during its deep public demo stage.

## User-visible reliability goals

From the user's perspective, reliability work is intended to support:

- consistent sign-in and session behavior;
- stable chat creation and history;
- predictable file uploads;
- streaming responses that fail cleanly when interrupted;
- clear handling of unavailable model capacity;
- safe API-key management in Studio;
- recovery from individual feature errors without exposing private internals.

## Deep-demo reality

SokSam AI is not presented as a finished, frozen product. Bugs and interface changes are still possible, and some capabilities are experimental or actively evolving.

The public project status is therefore intentionally transparent: usable today, but still under rapid development.

## Security boundary

Detailed internal security controls, test cases, thresholds, administrative access methods and infrastructure validation procedures are intentionally not documented publicly.

Security-sensitive reports should never be posted in a public GitHub issue. See [`../SECURITY.md`](../SECURITY.md) for reporting guidance.
