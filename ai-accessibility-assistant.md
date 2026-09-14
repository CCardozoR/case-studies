# AI Assistant for Accessibility Pitfalls

**Company:** Blackboard Inc. · **Role:** Senior Software Engineer · **Reach:** ~12 development teams, ~60 developers

## Problem

Blackboard's frontend surfaces (React + legacy AngularJS) have to meet WCAG accessibility
standards across a huge, varied feature set. Developers who weren't accessibility
specialists kept tripping over the same category of product-specific AX pitfalls —
patterns that are easy to get wrong unless you already know the product's own
conventions. Catching these in manual code review was too slow and too late: by the
time a reviewer flagged an issue, the developer had already built the feature the
wrong way.

## Constraints

- Couldn't scale by hiring more accessibility specialists — needed something developers
  could use themselves, in the moment, while they were writing code.
- Had to work across teams with very different day-to-day tooling and workflows.
- Had to be genuinely useful on the first try, or nobody would come back to it.

## What I built

I designed and shipped an internal, LLM-based assistant that developers could consult
while building frontend features, to flag the accessibility pitfalls specific to our
product before code ever reached review. It was the first tool of its kind adopted
company-wide — rolled out free to roughly 12 development teams (about 60 developers) —
and it measurably raised AX awareness across the product.

## Hardest part / what I'd do differently now

[ADD: what was the hardest part of building or rolling this out — getting teams to
adopt it, tuning it to avoid false positives, something else? And what would you
change if you built it again today? This is the section that makes the case study
sound like you, not like a resume bullet — write it in your own words.]

## Stack

LLM-based assistant, integrated into the frontend development workflow (Java/Spring
Boot + React/AngularJS product).

