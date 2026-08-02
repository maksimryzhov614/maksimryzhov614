# Mansara — Interactive residential experience

**Alpha case study · private source · local demo**

![Mansara interactive residential overview](../assets/case-studies/mansara-preview.webp)

## Summary

Mansara is an Alpha concept for exploring a residential complex through
approved visual source material. It connects an overview, facade choices,
floor selection, a sample apartment journey, and a park route in one responsive
browser experience.

## Problem

Architectural source material often arrives as separate renders, panoramas, and
video. The product challenge is to turn those inputs into a coherent journey
without suggesting more spatial precision or backend readiness than the
evidence supports.

## What I worked on

- A 120-image horizontal turntable with separate click and drag behavior,
  pointer and touch support, momentum, and reduced-motion handling.
- Organized nine stable facade views into clear building sections.
- Shared floor and apartment-tour state so the user keeps context while moving
  between the overview and deeper screens.
- A six-stop park walkthrough with still-image fallback behavior.
- Responsive navigation, keyboard-aware controls, asset checks, and interface
  states for loading and failure.

## System shape

The experience is a static browser application with a source-anchored
pseudo-3D presentation layer. Small data modules describe facade views, floors,
tour stops, and sample units; interface controllers keep URL and screen state
consistent across the journey.

## Reliability and verification

A local verification loop rebuilds the site, checks script syntax, validates UI
contracts, audits tour data and assets, and then hands off to a Google Chrome
smoke-test. The current Alpha passed that loop before the portfolio evidence was
captured.

## Current limitations

The experience uses demonstration data; CRM/API and real pricing are not
connected. It is source-anchored pseudo-3D: not continuous real-time 3D, a
spherical 360° model, CAD/BIM, or engineering-accurate geometry. The source is
private, and the profile does not publish a live link for this local Alpha. The
residential tour is a sample; office and retail tours are not available in this
Alpha.

## Evidence

- The overview image above is a fresh Google Chrome capture from the tested
  local Alpha, with no browser account or debugging interface included.
- The interaction and asset contracts pass the project's local verification
  loop.
- The portfolio intentionally presents the working boundary instead of
  implying a public deployment.

## Technology

JavaScript · HTML/CSS · Node.js verification · responsive browser media
