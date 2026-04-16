---
name: browse-awesome-skills
description: Searches the Awesome Claude Skills list to suggest skills, collections, authoring tools, or docs matching the user's need. Use when the user asks where to find a skill for a specific task, which collection is worth installing, or what the official Anthropic resources are.
allowed-tools: WebFetch
---

# Browse Awesome Skills

Help the user find the right entry in the [Awesome Claude Skills](https://github.com/horiastanxd/awesome-claude-skills) list.

## Steps

1. Fetch the latest list: `https://raw.githubusercontent.com/horiastanxd/awesome-claude-skills/main/README.md`
2. Read the user's request and figure out which section(s) apply: Official, Collections, Individual skills, Authoring tools, Reading & docs, or Related.
3. Suggest 1–3 entries that fit. For each, give the link and the one-line description from the list verbatim.
4. If nothing fits, say so. Don't invent entries.

## Guidelines

- Quote descriptions from the list verbatim; don't rewrite them.
- When recommending from Collections, mention whether the list is Claude-focused or multi-agent — that distinction is in the list itself.
- If the user wants to author a new skill, point to `skill-creator` first unless they need something more specific.
- If the request is about MCP servers or Claude Code plugins generally (not skills), point to the Related section, which cross-links to `awesome-mcp-servers` and `awesome-claude-code`.
- Link the section anchor when useful, e.g. `https://github.com/horiastanxd/awesome-claude-skills#collections`.

## Source

This skill is published alongside the list at https://github.com/horiastanxd/awesome-claude-skills. To add or correct an entry, open a PR there.
