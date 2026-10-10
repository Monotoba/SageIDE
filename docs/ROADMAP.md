# Sage IDE prototype roadmap

Status: proposed; no application implementation is present.

This roadmap narrows the original design into milestones that can be demonstrated and tested. It sets an implementation order, not a delivery date.

## 1. Local editor prototype

Proposed stack: Python and PyQt6, subject to dependency and license review before adoption.

Scope:
- A main window with a project directory view, tabbed plain-text editor, and status area.
- Open a local directory and UTF-8 text files; save and save as.
- Track unsaved changes and ask before closing or replacing edited content.
- Show readable errors for unsupported encoding, missing files, and write failures.

Acceptance:
- A documented command launches the prototype from a clean environment.
- Tests cover opening, editing, saving, cancellation, Unicode, and filesystem errors.
- A manual GUI checklist verifies keyboard navigation and unsaved-change prompts.
- No network requests or automatic command execution occur.
- CI validates the supported environment; other platforms remain explicitly unverified.

## 2. Testable extension interface

Define a minimal interface for registering an action and a panel. Start with one local example plugin.

Acceptance: tests verify registration, cleanup, and handling of plugin failures. Document that in-process plugins run with the application's permissions and are not sandboxed.

## 3. One reviewed AI workflow

Select one provider after evaluating its API, licensing, credentials, and data handling. Use a mocked provider for repeatable tests before live integration.

Scope: user selects context, submits a request, and reviews a suggested patch. No automatic edits or shell commands.

Acceptance: tests cover cancellation, timeouts, authentication failures, response handling, and patch rejection. Document what leaves the machine and how credentials are stored.

## 4. Alpha release gate

Publish an application alpha only after the first runnable workflow is documented and validated. Include installation instructions, supported platforms, test results, known limitations, and screenshots. Keep provider integrations and broader agent roles clearly separated from implemented features.

The roles, broad plugin powers, packaging targets, and multiple integrations in the original design remain later proposals until these milestones are evaluated.
