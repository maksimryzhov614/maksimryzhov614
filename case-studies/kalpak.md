# kalpak.dev — Storefront bureau for Telegram shops

**Production case study · private source · live product**

![kalpak.dev landing hero with large typography on a dark background](../assets/case-studies/kalpak-preview.webp)

## Summary

**Role:** Full product engineering and design: concept, UI, motion, content
honesty rules, and the release verification pipeline.

kalpak.dev is the storefront of a bureau that turns Telegram catalog channels
into ordering websites: Telegram catalog in, a clear site out, orders routed
back to the channel. The site is itself the product demo: it shows one real
client project, clearly labeled demo concepts, eight switchable design
directions, and tiered service packages.

## Problem

Selling web development honestly is harder than selling it loudly. The
storefront has to demonstrate range without inventing clients, separate a
real production project from concept work explicitly, and still feel like a
designed product rather than a template.

## What I worked on

- A dark editorial landing with large display typography and GSAP-driven
  motion, built on Next.js React Server Components.
- A projects grid where the single real project (Tunika) is labeled
  «реальный проект» and every concept card is labeled «демо-концепт, не
  клиентский проект» — the honesty rule is part of the interface.
- An interactive showcase of eight design directions (Swiss Grid, Editorial
  Cut, Quiet Luxury, Commercial Brutalism, Future Systems, Soft Organic,
  Kinetic Color, Modern Commerce) rendered as live desktop and mobile
  mockups.
- Service tiers for control, maintenance, and growth, priced by level of
  responsibility rather than by the hour.
- Delivery on Cloudflare Workers through a Vite RSC build.

## Reliability and verification

The repository ships with contract and runtime tests in Playwright, mobile
Lighthouse budgets, dependency and security audit scripts, and release
verification steps that sanitize the built output before it is published.

## Outcome

- The bureau has a live, self-demonstrating storefront where the design
  range is shown by the site itself, not by claimed portfolios.
- Real work and concept work are visibly separated, so a prospect never
  mistakes a demo for a client reference.

## Current limitations

The source is private because this is an active commercial storefront. The
demo concepts intentionally represent no existing businesses.

## Evidence

- [Live site](https://kalpak.dev/)
- The hero image above was captured from the public landing page in Google
  Chrome after confirming that the page loaded correctly.

## Technology

TypeScript · Next.js (React Server Components) · React · GSAP · Vite ·
Cloudflare Workers · Playwright · Lighthouse
