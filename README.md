# DivineDesk CRM Case Study

Private source repository. Public portfolio case study.

![DivineDesk dashboard preview](assets/mockups/dashboard.svg)

## Overview

DivineDesk is a church-management CRM designed for congregations that need one organized workspace for people, families, groups, attendance, giving, communications, reports, and daily operations.

The project is built on the open-source ChurchCRM foundation and reworked into a calmer, branded product experience. My work focused on product positioning, frontend presentation, release packaging, local run documentation, and keeping the ChurchCRM compatibility boundary intact.

## My Role

Product engineer and full-stack implementer.

- Rebranded the application as DivineDesk while preserving ChurchCRM-compatible internals.
- Organized the product story around practical church operations rather than generic CRM language.
- Worked on release packaging and Docker-based local setup documentation; a reproducible reviewer release remains to be verified.
- Maintained a privacy-conscious split between private source code and public portfolio evidence.
- Documented the architecture, technology decisions, validation commands, and user-facing workflows.

## Problem

Church teams often need operational software that is useful without feeling like enterprise sales tooling. The system had to keep proven ChurchCRM capabilities while making the product feel simpler, warmer, and more credible for non-technical church administrators.

## Solution

DivineDesk keeps the robust ChurchCRM core and presents it through a more focused product layer:

- People and family records for pastoral care and administration.
- Groups, ministries, classes, attendance, and check-in workflows.
- Events, calendars, kiosk flows, and communication tools.
- Giving, pledges, deposits, and finance reports.
- Plugin-compatible architecture and localization support.

## Interface mockups

These SVG illustrations show representative UI and synthetic figures. They are not browser captures or evidence of production usage. Real demo captures and a reproducible release are follow-up work.

### Operations Dashboard

![Dashboard mockup](assets/mockups/dashboard.svg)

### People And Families

![People directory mockup](assets/mockups/people-directory.svg)

### Member Profile

![Member profile mockup](assets/mockups/member-profile.svg)

### Ministry Operations

![Ministry operations mockup](assets/mockups/ministry-operations.svg)

## Technical Highlights

- PHP application architecture with ChurchCRM-compatible namespaces and routes.
- JavaScript and TypeScript asset pipeline using Webpack.
- Bootstrap 5 and Tabler-inspired interface patterns.
- Docker-based local setup guidance for future reviewer demos.
- MySQL-backed CRM domain model with people, family, group, finance, event, and admin workflows.
- Localization-ready structure for multilingual church communities.

## Engineering Decisions

### Preserve Compatibility

Visible branding says DivineDesk, while internal technical identifiers remain ChurchCRM-compatible where they affect routes, APIs, database tables, generated assets, or ecosystem compatibility.

### Keep Source Private

The source repository is private because it contains the full application implementation and release workflow. This public repository is intentionally a case study: it shows the product, decisions, mockups, and technical depth without exposing private source code.

### Make Local Review Possible

A reviewer demo should use synthetic data in an isolated local environment. A downloadable, verified release package is not currently provided through this case study.

## Validation

The project includes standard validation commands for the private codebase:

```bash
npm run lint
npm run build:webpack
npm run build
```

These are verification commands, not a claim of passing results. At the 14 September 2026 repository review, no tracked `dist/DivineDesk-7.4.0` package or `DivineDesk-7.4.0-shareable.zip` was found, and the repository's Releases list was empty. Any package held outside GitHub must be verified and made available through an approved review route before it is advertised here.

## Attribution

DivineDesk is built on the open-source ChurchCRM project. This case study describes the DivineDesk product layer, packaging, and portfolio presentation work while respecting the upstream project foundation.
