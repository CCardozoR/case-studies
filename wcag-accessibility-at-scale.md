# WCAG Accessibility Compliance at Scale

**Company:** Blackboard Inc. · **Role:** Senior Software Engineer · **Domain:** Communications & Collaboration (Discussions)

## Problem

Blackboard's Discussions feature is used across 150M+ users in 80+ countries, which
means accessibility isn't optional — it's a legal and product requirement across many
jurisdictions. I was the lead engineer for WCAG conformance in this domain, responsible
for finding and closing accessibility gaps on an ongoing basis, not just at launch.

## Constraints

- A continuously evolving feature set — new UI shipping constantly, each capable of
  introducing new accessibility regressions.
- A mix of legacy AngularJS and modern React code, each with different accessibility
  tooling and idioms.
- Needed a sustainable cadence, not a one-time audit — accessibility debt accumulates
  quietly if nobody owns it.

## What I did

I owned accessibility compliance for the domain end-to-end: auditing, triaging, and
fixing issues, and setting the standard other engineers' code was reviewed against.
Over about two years, this meant consistently finding and resolving 4-6 accessibility
defects per quarter, ranging from critical (blocking assistive technology) to minor
(nice-to-have improvements). This sustained, unglamorous work contributed to the
highest internal AX (accessibility) score in the product line.

## Hardest part / what I'd do differently now

The genuinely hard part wasn't fixing individual defects — it was building the awareness that accessibility needs to enter the development cycle at the very first steps, not get bolted on at the end as a review-stage checklist item. Shifting that mindset across a fast-shipping team took sustained, repeated effort, not a single training or a one-off audit.

That shift paid off in two ways: it improved formal compliance, which is easy to measure, but it also improved the product's overall UX in ways that are much harder to track at a small scale — the kind of intangible quality that's hard to point to in a single metric but is genuinely part of what makes a product feel great to use. If I were setting the program up again, I'd try to find a way to make that second, harder-to-measure benefit visible earlier, since it's the stronger argument for why accessibility deserves a seat at the design table rather than just a pass before ship.

## Stack

Java, Spring Boot, PostgreSQL (backend) · React, TypeScript, AngularJS (frontend) ·
WCAG / AX tooling and manual audits
