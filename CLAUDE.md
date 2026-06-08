# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Business planning documents for **summer-buiz**, a 3-person web agency building clean websites for local businesses. The team is Owen (CEO & tech lead — builds sites with Claude Code), Connor (co-builder — code review and technical problem solving), and Ryan (sales lead — client pitches and content validation).

The repo currently contains a single file (`summer_agency_business_plan.html`) — a self-contained HTML fragment with no build step, no framework, and no dependencies.

## File structure

- `summer_agency_business_plan.html` — the entire plan as a styled HTML fragment. Uses CSS custom properties (`var(--color-*)`, `var(--font-sans)`, etc.) that are injected by the host environment (e.g. Claude's artifact renderer or a parent page). Tabler Icons (`ti ti-*`) are loaded externally.

## Editing conventions

- The file is a fragment, not a full HTML document — no `<html>`, `<head>`, or `<body>` tags.
- CSS lives in the single `<style>` block at the top of the file.
- Layout uses CSS Grid (`grid-4`, `grid-3`, `grid-2`) with `auto-fit` columns — add new grid items by duplicating sibling elements inside the same grid container.
- Color tokens (`--color-text-primary`, `--color-background-secondary`, etc.) and border-radius tokens (`--border-radius-lg`, etc.) come from the host environment — do not hardcode hex colors for structural elements; use tokens. Brand/accent colors (the pill and metric accent colors) are hardcoded hex and can be changed freely.

## Business context (for content edits)

| Role | Person | Owns |
|------|--------|------|
| CEO & Tech Lead | Owen | Claude Code builds, GitHub, Vercel, Stripe, client comms |
| Co-builder | Connor | Code review, technical problem solving |
| Sales Lead | Ryan | Client pitches, content validation |

**Target clients:** local gyms, restaurants, barbershops, coaches.

**Pricing:** $300–$800 one-time site build + $75–$150/month maintenance retainer.

**Tech stack:**
- Claude Code — primary builder
- VS Code — code review and manual edits
- GitHub — version control; each client site is its own separate repo
- Vercel — deployment; each client site is its own separate Vercel project
- Stripe — one-time build payments and recurring monthly retainer billing
