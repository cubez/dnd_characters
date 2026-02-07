# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a **D&D character reference repository** — a collection of markdown-based quick-reference sheets designed to be browsed on a phone during play sessions. There is no build system, no tests, and no application code. The repo is pure markdown documentation.

## Structure

- `README.md` — index page listing all characters with links
- `<CharacterName>/` — one directory per character, each containing:
  - `README.md` — character landing page with navigation table
  - `stats.md` — ability scores, AC, saves, skills, attacks, spell slots, feats, resources
  - `combat.md` — combat decision flowcharts and turn structure
  - `abilities.md` — detailed spell and ability descriptions with usage guidance
  - `quick-reference.md` — single-page summary of key numbers and actions
  - `flavor.md` — roleplay notes, personality, exploration utility, one-liners

## Conventions

- All pages use **internal relative links** for navigation (e.g., `[Combat Cheat Sheet](combat.md)`)
- Every page includes a back-link to its character README and cross-links to sibling pages
- Tables use GitHub-flavored markdown with center-aligned numeric columns (`:---:`)
- Spells/abilities follow a consistent format: name, source/type, action cost, range, duration, then "When I use this" / "What this does" / "If I use this" / "Reminder" sections
- Combat pages use a **situation-based decision tree** pattern, not exhaustive option lists
- The tone is second-person practical ("When I use this...", "Never do this...")

## When Adding a New Character

1. Create a new directory named after the character
2. Add the character to the root `README.md` index
3. Create all five reference files (README, stats, combat, abilities, quick-reference, flavor) following the existing structure
4. Ensure all internal cross-links work
