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

[ADD: what was the trickiest part of this from the frontend side — handling
imperfect AI-generated chapter suggestions gracefully in the UI, performance,
something else? And what would you do differently if you built it again?]

## Stack

React, TypeScript (frontend) · Spring Boot APIs (backend, AI/ML pipeline)
