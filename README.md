# Sage IDE

![Status: design stage](https://img.shields.io/badge/status-design%20stage-orange)
![Implementation: planned](https://img.shields.io/badge/implementation-planned-lightgrey)
[![License: MIT with notice](https://img.shields.io/badge/license-MIT%20with%20notice-blue)](LICENSE)

Sage IDE is a proposed desktop development environment that brings AI assistance into requirements, design, coding, testing, and documentation. The goal is to let developers review agent suggestions alongside their project files, with explicit control over changes.

**This repository currently contains design documents and RFCs only.** There is no runnable IDE, implemented AI integration, installer, application test suite, or published application release. Python and PyQt6 are proposed implementation choices.

## Explore the proposal

- [Design overview](docs/design-overview.md): original architectural proposal, with its historical context.
- [Prototype roadmap](docs/ROADMAP.md): a small first milestone and acceptance criteria.
- [Introducing Sage IDE](RFC/rfc-00001.md): initial request for comments.
- [RFC process](RFC/RFC_PROCESS.md) and [RFC template](RFC/RFC_TEMPLATE.md): how to propose changes.

The original design names ChatGPT, ChatDev, and Aider as candidate integrations. These are ideas to evaluate, not working integrations or promises of compatibility.

## Help shape the first prototype

Useful contributions include reviewing the editor workflow, narrowing the plugin interface, defining tests, and identifying privacy and permission requirements for AI tools. No AI account or API key is needed to review the design.

Read [CONTRIBUTING.md](CONTRIBUTING.md), then [open an issue](https://github.com/Monotoba/SageIDE/issues) with a concrete use case or submit a focused documentation pull request. Please explain the problem, expected behavior, and how your proposal could be tested.

## Project status and validation

The next proposed milestone is a local editor prototype without network access or agent execution. Application CI and build badges will be added when there is an implementation to validate. At this stage, review checks focus on documentation accuracy and repository links.

## License and conduct

The current [LICENSE](LICENSE) contains the MIT terms and an additional third-party licensing notice; it is retained unchanged. Future dependencies require their own license review.

Follow the [Code of Conduct](CODE_OF_CONDUCT.md). Its reporting contact is documented there.
