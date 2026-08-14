# ART SQUARE STUDIO — Multilingual studio site

**Production case study · private source · live product**

![ART SQUARE STUDIO landing page with a 1:100 architectural scale model](../assets/case-studies/artsquare-preview.webp)

## Summary

**Role:** Full product engineering: architecture, UI, content system, security headers, and the release verification pipeline.

ART SQUARE STUDIO is the production website of an architectural scale-model
and digital development studio. The site presents the studio's two service
directions, a curated project portfolio, and a contact flow, and it ships in
four production locales: Russian, English, Kyrgyz, and German.

## Problem

A small studio site still has production-grade obligations: every page must
exist in four locales without drift, portfolio claims must stay verifiable,
legal and consent texts must be present, and each release must be provably
safe to publish rather than assumed to be.

## What I worked on

- Next.js App Router architecture with locale-prefixed routes (`ru`, `en`,
  `ky`, `de`), service-direction pages, project pages, and legal pages with
  deliberate indexing rules.
- A single-source content system where all site copy lives in one typed
  module, with an automated gate that fails the release if any locale is
  missing a key.
- A strict nonce-based Content-Security-Policy generated from one source and
  issued per request, plus contact-form consent handling.
- Observability adapters for Sentry and ntfy that stay no-op unless
  explicitly configured, so the site collects nothing by default.

## Release verification

One command runs the entire pre-release pipeline: 13 checks that stop at the
first failure. They cover dependency audit, CSP and locale contracts, consent
and legal texts, robots and sitemap, the canonical domain, a license
registry, the full route matrix, accessibility, Lighthouse budgets, and a
real Safari pass through safaridriver. Every run writes its evidence to the
repository so a reviewer can inspect what was actually verified.

## Outcome

- The site is live in four locales with enforced copy parity: a missing
  translation key is a failed release, not a silent gap.
- Security and privacy defaults are verified on every release: strict
  nonce-based CSP, telemetry off unless configured, and legal pages checked
  by the gate.
- Publication is evidence-based: each release leaves an inspectable record of
  the 13 checks it passed.

## Current limitations

The source is private because this is an active commercial product. The
screenshot shows only the public landing page; client project data beyond the
approved portfolio is intentionally excluded.

## Evidence

- [Live site](https://art-square.studio/)
- The interface image above was captured from the public landing page in
  Google Chrome after confirming that the page loaded correctly.
- The described release pipeline is backed by scripted gates whose evidence
  is committed alongside each release.

## Technology

TypeScript · Next.js · React · Node.js · Playwright · Lighthouse ·
safaridriver · Cloudflare
