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

[ADD: what made this hard in practice — sequencing the refactor so nothing broke,
convincing stakeholders to invest time in it, a specific piece of the old design
that was especially painful to untangle? And anything you'd sequence differently
if you did it again?]

## Stack

Java, Spring Boot, PostgreSQL, microservices architecture
