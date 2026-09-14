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

The hardest part wasn't the tooling — it was distilling years of accumulated, tribal knowledge about our product's specific accessibility pitfalls into a single, thorough document that was precise enough for an LLM to act on reliably. Too vague and it produced noise; too narrow and it missed real cases. Getting that balance right took real iteration.

The other hard part was adoption reach. A written skill only helps if it's actually consulted, so I pushed it into two different moments in the workflow rather than leaving it as a document people had to remember to open: first into automated code review, where it caught AX issues an LLM could flag from the diff even when they'd slip past a human reviewer's attention; and later into early design conversations, so accessibility got discussed before a single line of frontend code was written instead of after. That second move — shifting the AX conversation left, into design — is what actually changed behavior across teams, more than the code-review catch rate did.

If I did it again, I'd build a tighter feedback loop from day one: a way for developers to flag a missed or wrong pitfall straight back into the document, so it improved from real usage instead of periodic manual updates from me.

## Stack

LLM-based assistant, integrated into the frontend development workflow (Java/Spring
Boot + React/AngularJS product).

