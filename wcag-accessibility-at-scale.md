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

[ADD: what was genuinely hard about this — getting other engineers to care about
accessibility before it broke something, keeping up with a fast-shipping team,
some specific defect that was gnarly to fix? And is there anything about how the
program was run that you'd change if you were setting it up again?]

## Stack

Java, Spring Boot, PostgreSQL (backend) · React, TypeScript, AngularJS (frontend) ·
WCAG / AX tooling and manual audits
