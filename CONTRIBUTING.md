# Contributing to Sage IDE

Sage IDE is in the design stage. Contributions should help turn the proposal into a small, testable prototype.

## Start with a concrete problem

Review the [README](README.md), [design overview](docs/design-overview.md), and [roadmap](docs/ROADMAP.md). Open an issue describing a developer task, the proposed behavior, and an observable acceptance criterion. For architectural changes, use the [RFC process](RFC/RFC_PROCESS.md).

Good first contributions include correcting documentation, reviewing the first editor milestone, and proposing tests for file handling and unsaved changes. Keep each pull request focused and preserve unrelated content.

## Documentation changes

Check spelling, relative links, and consistency between proposed and implemented features. Mark unimplemented behavior as proposed. Avoid claiming performance, reliability, compatibility, or integrations without evidence.

## Future code contributions

Once implementation begins, prefer small refactorings over rewrites. Include tests for every code change, including failure cases. Describe the validation performed in the pull request and commit changes with a clear message.

The prototype should work offline. Never commit credentials, private project files, or personal data. AI requests and file changes must be designed for explicit user control before provider integrations are introduced.

## Review and conduct

A proposal or pull request does not imply that its design has been accepted. Maintainers review scope, testability, and compatibility with the roadmap before implementation.

Follow the [Code of Conduct](CODE_OF_CONDUCT.md). The repository's [license](LICENSE), including its third-party notice, remains unchanged.
