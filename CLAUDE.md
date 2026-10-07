# CLAUDE.md — Default theme

This repo is one pack of [Ostler](https://github.com/openostler/ostler/blob/main/README.md), an Android-style OS for cars:
the platform repo `openostler/ostler` is the bare system, and every feature is an app or
pack in its own repo ([ADR-0046](https://github.com/openostler/ostler/blob/main/decisions/adr-0046-empty-os-every-app-an-add-on.md)).

## Read first

- The platform [CONSTITUTION](https://github.com/openostler/ostler/blob/main/CONSTITUTION.md): its hard rules apply here too.
- [ADR-0045, UX first](https://github.com/openostler/ostler/blob/main/decisions/adr-0045-ux-first.md) and [ADR-0046](https://github.com/openostler/ostler/blob/main/decisions/adr-0046-empty-os-every-app-an-add-on.md).
- This repo's design brief and spec, linked from [README.md](README.md).

## Working rules

- UX first (platform ADR-0045): no screen, setup flow or widget without an approved UX
  brief; build it against recorded fixtures before wiring. Decoding, protocol and pack-data
  work need no brief.
- Safety stays in the OS: Moving templates, Park to edit, alarm alerts and the fault
  telltale are never this repo's to change.
- No demo data: recorded fixtures only (platform ADR-0011).
- Never put model or AI product names in repo content.
- One PR per change; it merges when CI is green.
