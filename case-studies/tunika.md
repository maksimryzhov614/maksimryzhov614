# Tunika — Production commerce platform

**Production case study · private source · live product**

![Tunika production catalog interface](../assets/case-studies/tunika-preview.webp)

## Summary

**Role:** Product engineering across responsive UI, catalog publication, operational safeguards, and release verification.

Tunika is a live fabric commerce platform for catalog discovery, product
selection, and operationally reliable publication. My contribution covers
defined engineering areas inside a broader retail product: responsive customer
interfaces, browser media behavior, catalog delivery, and release safeguards.

## Problem

A fabric catalog has to keep customer-facing product data, media variants, and
back-office state aligned without publishing partial or misleading results.
The interface also has to remain usable across real desktop and mobile
viewports while the catalog changes underneath it.

## What I worked on

- Responsive catalog and product-page behavior, including filters, sorting,
  badges, fabric-unit presentation, and short mobile viewports.
- Browser-selected product media with JPG, WebP, and AVIF variants and checks
  for missing or undecodable assets.
- Go-backed catalog publication and MoySklad reconciliation behavior for
  product visibility and availability changes.
- Release verification that checks the public interface, not only source files
  or back-office records.

## System shape

The browser UI consumes a published catalog and its generated media variants.
A Go application coordinates catalog generation and reconciliation with
MoySklad. Publication steps connect those layers while keeping a clear boundary
between generated output and the currently served version.

## Reliability and verification

Publication uses fail-closed checks so an incomplete build does not silently
replace a known-good catalog. The delivery process includes separate backups,
rollback points, focused automated tests, and browser-visible checks at desktop
and real mobile viewports. Operational fixes are verified against the public
product experience after deployment.

## Current limitations

The source is private because this is an active commercial product. This case
study describes my scoped contribution rather than claiming ownership of the
entire business or codebase. The screenshot contains only the public catalog
interface; internal operations and exact business metrics are intentionally
excluded.

## Evidence

- [Live Tunika catalog](https://tunika-tkani.ru/)
- The interface image above was captured from the public catalog in Google
  Chrome after confirming that the page loaded correctly.
- The described delivery work is backed by focused automated checks and
  browser-visible release acceptance.

## Technology

Go · JavaScript · HTML/CSS · Playwright · Linux delivery automation · MoySklad
