# Incremental Monolith Refactor

**Company:** Blackboard Inc. · **Role:** Senior Software Engineer · **Stack:** Java, Spring Boot, PostgreSQL, microservices

## Problem

A large, long-lived Java/Spring Boot monolith, integrated with a growing set of
microservices, had become expensive to extend. Before this work, shipping a new
feature into the monolith routinely took a full quarter — the codebase's structure
worked against incremental change, so every addition meant fighting the existing
design rather than building on it.

## Constraints

- The monolith was live, serving a product used by 150M+ users — a disruptive,
  stop-the-world rewrite was not an acceptable option.
- Needed to keep shipping product features on the existing system while the
  refactor was happening, not pause the roadmap to do it.
- Had to bring the rest of the team along, since a refactor only pays off if
  people actually build on the new structure afterward.

## What I did

I defined and executed an incremental refactoring strategy for the monolith,
restructuring it piece by piece alongside the microservices it was already
integrated with — without a disruptive full rewrite. The result: delivery time
for new functionality dropped from a full quarter to about a week.

## Hardest part / what I'd do differently now

The hardest part wasn't technical — it was convincing stakeholders to accept one big, predictable pain up front instead of the alternative: a long tail of small, unpredictable pains that would keep cascading into rework and slower delivery every quarter after. That meant making the case to sacrifice visible feature delivery for a couple of sprints in order to guarantee the team's productivity for the next couple of quarters — a hard trade to sell when the cost is immediate and concrete and the payoff is diffuse and in the future.

If I did it again, I'd invest earlier in making that future payoff visible and trackable — instrumenting delivery time before the refactor started, so the "quarter to a week" result wasn't just a story I told afterward but a number stakeholders could watch materialize in real time, which would make the next case for this kind of trade-off easier to make.

## Stack

Angular JS, React 
