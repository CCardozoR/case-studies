# AI-Powered Video Analysis Feature

**Company:** Blackboard Inc. · **Role:** Senior Software Engineer · **Stack:** React, Spring Boot

## Problem

Long-form video content on the platform was hard to navigate — students and
instructors had no quick way to find the part of a video they actually needed,
short of scrubbing through the whole thing manually.

## Constraints

- The feature needed to work across a huge existing catalog of video content,
  not just newly uploaded videos.
- Frontend needed to feel instant even though the underlying analysis is
  computationally heavier than a typical UI interaction.
- Had to fit into the existing React component architecture and consume
  whatever the backend AI/ML pipeline produced, without the frontend needing
  to know the internals of that pipeline.

## What I built

I built the React frontend for an AI-powered video analysis feature, consuming
Spring Boot APIs to auto-generate timestamps and chapter suggestions for video
content. This gave users a way to jump directly to the relevant section of a
video instead of scrubbing manually, improving content navigation and overall
usability of long-form video.

## Hardest part / what I'd do differently now

The trickiest part wasn't wiring the frontend to the AI-generated output — it was the interaction design itself. Chapter markers and jump-to-timestamp navigation are patterns people take for granted now, but at the time there wasn't an established, off-the-shelf pattern to copy for this product. I had to design the interaction from scratch: how imperfect, AI-generated suggestions should present themselves in the UI, how a user scans and trusts a set of auto-generated chapters, how the whole thing degrades gracefully when a suggestion is mediocre rather than wrong.

What I'd do differently now: apply the accessibility expertise I've built since then to that same interaction design. At the time I was solving for the general case; today I'd design the chapter navigation to genuinely work for a wider audience — screen reader users, keyboard-only navigation, users with different visual and cognitive needs — from the first version, rather than treating that as a pass to layer on afterward.
## Stack

React, TypeScript (frontend) · Spring Boot APIs (backend, AI/ML pipeline)
