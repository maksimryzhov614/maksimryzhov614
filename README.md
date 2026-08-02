# Maksim Ryzhov

**Frontend / Full-stack Product Engineer**

I build reliable interactive web products and developer tools, with tests,
automation, and explicit privacy boundaries.

## Selected work

### [Viewport Sentinel](https://github.com/maksimryzhov614/viewport-sentinel)

A Chromium CLI and GitHub Action for catching responsive and browser-media
regressions before release.

- Audits an explicit page-by-viewport matrix for overflow, covered controls,
  browser-selected image failures, and browser runtime errors.
- Produces deterministic JSON and SARIF reports through a tested fail-last
  Action workflow.
- Ships with 327 automated tests and a reproducible Node 22/24/26 CI matrix.

[CI](https://github.com/maksimryzhov614/viewport-sentinel/actions/workflows/ci.yml)
· [v0.1.0](https://github.com/maksimryzhov614/viewport-sentinel/releases/tag/v0.1.0)
· [npm](https://www.npmjs.com/package/viewport-sentinel/v/0.1.0)
· [demo](https://github.com/maksimryzhov614/viewport-sentinel/blob/main/docs/assets/demo.gif)

### [Hermes Agent for VS Code](https://github.com/maksimryzhov614/hermes-vscode)

A VS Code client for a self-hosted agent bridge, designed around reviewable
context and code-edit workflows.

- Attaches files, editor selections, and screenshots to agent conversations.
- Turns structured edits into native review/apply diffs with explicit modes.
- Provides a downloadable VS Code extension through an automated public
  release workflow.

[v0.10.1 release](https://github.com/maksimryzhov614/hermes-vscode/releases/tag/v0.10.1)
· [source](https://github.com/maksimryzhov614/hermes-vscode)

## Engineering approach

- Make verification reproducible before calling work complete.
- Keep privacy, failure behavior, and product limitations explicit.
- Prefer focused tools and maintainable delivery paths over feature volume.

## Core tools

TypeScript · JavaScript · Node.js · Playwright · GitHub Actions
