# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

A documentation repository for a solo D&D 5e campaign (2024 PHB rules, Forgotten Realms setting) where Claude serves as DM. No build system, tests, or code — all files are Markdown.

The core workflow: update relevant docs → upload to Claude Project → play session → commit DM-generated session recap and updated docs.

## Document Roles

- **system-prompt.md** — Paste into the Claude Project instructions field before sessions. This is the DM's operating charter.
- **character/zero-sheet.md** — Source of truth for Zero's current stats, spells, equipment, and currency. Update after every session.
- **session/session-log.md** — Campaign ground truth. The Current State block at the top must stay current; never delete old session entries.
- **session/quest-tracker.md** — Active and completed quests; update when quest status changes.
- **party/npc-roster.md** — Full stat blocks for companion NPCs. Add entries when a companion joins the party.
- **party/npc-directory.md** — Quick-reference table for every NPC encountered. Add a row after each new NPC interaction.
- **world/factions-reputations.md** — Tracks Zero's standing with each faction. Update when reputation changes.
- **world/locations-visited.md** — Log significant locations as they're explored.
- **rules/house-rules.md** — Specific 2024 PHB rulings and DM preferences. Add entries when a ruling is made mid-session.

## Key Campaign Rules

- System: D&D 5e **2024 PHB** (not 2014). When rules questions arise, default to 2024 PHB, then check `rules/house-rules.md` for campaign-specific rulings.
- Leveling: Milestone (narrative), not XP.
- Death saves: RAW for major NPCs; other NPCs die at 0 HP.
- No fudging dice outcomes. Real consequences matter.
- Zero's spellcasting: Charisma-based, DC 13, attack +5.

## Character: Zero (Current State)

Level 3 Changeling Bard (College of Lore), Charlatan background, they/them. Key numbers: HP 24, AC 14, Initiative +3, Bardic Inspiration 3×/long rest (d6). Expertise in Deception and Persuasion (+7). See `character/zero-sheet.md` for full details.

## Editing Guidelines

- **Accuracy over completeness.** Stats and rules must match the 2024 PHB exactly. Prior commits show errors were introduced and had to be corrected from the PDF source — always verify against source material.
- The session log is append-only for past sessions. Only the Current State block at the top gets overwritten each session.
- Templates in `party/` and `session/` are pre-structured — preserve their format when adding entries.
- Currency in zero-sheet.md is tracked in cp/sp/gp separately; don't collapse into gold.
