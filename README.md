# Maksim Ryzhov

**Frontend / Full-stack Product Engineer**

I build reliable interactive web products and developer tools, with tests,
automation, and explicit privacy boundaries.

## Product work — Alpha case studies

These private-source case studies show product engineering work with explicit
scope and evidence boundaries. They are not presented as open-source repos.

### Tunika — Production commerce platform

**Alpha case study · private source · live production**

A live fabric catalog where I work across customer-facing UI and the delivery
path behind reliable catalog updates.

- Built responsive catalog and product interfaces, including browser-selected
  media behavior.
- Worked on Go-backed publication and MoySklad reconciliation paths.
- Added fail-closed checks, backup and rollback discipline, and browser-visible
  release verification.

[Read the case study](https://github.com/maksimryzhov614/maksimryzhov614/blob/main/case-studies/tunika.md)
· [Live site](https://tunika-tkani.ru/)

### Mansara — Interactive residential experience

**Alpha case study · private source · local demo**

A source-anchored interactive concept for exploring a residential complex,
facades, floors, and a sample apartment journey.

- Built a 120-image horizontal turntable with pointer and touch interaction.
- Organized nine stable facade views around shared floor and tour state.
- Added responsive controls, fallbacks, and a six-stop park walkthrough.

[Read the case study](https://github.com/maksimryzhov614/maksimryzhov614/blob/main/case-studies/mansara.md)

## Developer tools

### [Viewport Sentinel](https://github.com/maksimryzhov614/viewport-sentinel)

A Chromium CLI and GitHub Action for catching responsive and browser-media
regressions before release.

- Audits an explicit page-by-viewport matrix for overflow, covered controls,
  browser-selected image failures, and browser runtime errors.
- Produces deterministic JSON and SARIF reports through a tested fail-last
  Action workflow.
- Ships with 328 automated tests and a reproducible Node 22/24/26 CI matrix.

[CI](https://github.com/maksimryzhov614/viewport-sentinel/actions/workflows/ci.yml)
· [v0.1.1](https://github.com/maksimryzhov614/viewport-sentinel/releases/tag/v0.1.1)
· [npm](https://www.npmjs.com/package/viewport-sentinel/v/0.1.1)
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
