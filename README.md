# Awesome Claude Skills [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A list of Skills for [Claude](https://claude.com) - the instruction packages (SKILL.md + optional scripts) that extend Claude Code and the Claude apps.

Skills were introduced by Anthropic in October 2025. Claude only loads a skill's body when it looks relevant, so you can install a lot of them without bloating context.

Here you'll find the official repos, community collections, standalone skills worth installing on their own, tools for authoring, and the handful of posts and docs that are actually useful.

## Contents

- [Official](#official)
- [Collections](#collections)
- [Individual skills & skill-based plugins](#individual-skills--skill-based-plugins)
- [Authoring tools](#authoring-tools)
- [Reading & docs](#reading--docs)
- [Related](#related)
- [Use this list as a skill](#use-this-list-as-a-skill)
- [Contributing](#contributing)

## Official

- [anthropics/skills](https://github.com/anthropics/skills) - The reference repo. Source of the built-in docx/pdf/pptx/xlsx skills, the `skill-creator`, the spec, and a template to copy from.
- [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) - Anthropic's managed plugin directory. Many plugins here bundle skills; `/plugin install <name>@claude-plugins-official` in Claude Code.
- [anthropics/claude-cookbooks - skills/](https://github.com/anthropics/claude-cookbooks/tree/main/skills) - Notebooks: intro, financial workflows, and a walk-through of building a skill end-to-end.
- [agentskills/agentskills](https://github.com/agentskills/agentskills) - Open Agent Skills spec and reference SDK. Includes `skills-ref`, the validator most skill authors end up using.

## Collections

Claude-focused:

- [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) - Large list with ~78 SaaS-workflow skills (CRM, DevOps, analytics). Well-organized.
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) - Broader Claude Code list. Overlaps with skills but also covers hooks, slash commands, and plugins.
- [travisvn/awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills) - Claude-specific, emphasis on Claude Code workflows.
- [BehiSecc/awesome-claude-skills](https://github.com/BehiSecc/awesome-claude-skills) - 200+ skills across 13 categories.
- [jeremylongshore/claude-code-plugins-plus-skills](https://github.com/jeremylongshore/claude-code-plugins-plus-skills) - Very volume-heavy: 340 plugins + 1367 skills, packaged with a CCPI installer. Quality varies.
- [rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit) - Toolkit-style: skills, agents, commands, hooks, templates, MCP configs, and companion apps.
- [daymade/claude-code-skills](https://github.com/daymade/claude-code-skills) - 48 production skills. Ships a hardened fork of `skill-creator`.
- [abubakarsiddik31/claude-skills-collection](https://github.com/abubakarsiddik31/claude-skills-collection) - 173 catalogued skills with an index-style layout.
- [simonw/claude-skills](https://github.com/simonw/claude-skills) - Simon Willison's original extraction of `/mnt/skills` from Claude's code interpreter. Mostly of historical interest now that the official repo exists.

Multi-agent (work with Claude alongside Codex, Cursor, Gemini CLI, and others):

- [sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills) - 1400+ skills with an installer CLI and pre-built bundles.
- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) - 1000+ skills organized by provider. Good if you're mixing tools.
- [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) - 232+ skills across engineering, marketing, product, compliance, and C-level advisory. Works on 12 coding agents.
- [DeadInternetStudios/100x-engineer-skill](https://github.com/DeadInternetStudios/100x-engineer-skill) - 13 skills for planning agent work first and verifying it with tests and formal checks.

## Individual skills & skill-based plugins

Single-purpose repos worth installing on their own.

- [obra/superpowers](https://github.com/obra/superpowers) - Jesse Vincent's skills-based workflow (brainstorm → plan → TDD → review). Probably the most influential single skills release to date.
- [obra/superpowers-marketplace](https://github.com/obra/superpowers-marketplace) - Plugin marketplace that bundles Superpowers with extras like Elements of Style, Private Journal MCP, and Episodic Memory.
- [obra/superpowers-skills](https://github.com/obra/superpowers-skills) - Community-editable skill pack for the Superpowers plugin. Archived in late 2025 but still a good reference.
- [obra/superpowers-lab](https://github.com/obra/superpowers-lab) - Experimental companion: new techniques that haven't landed in Superpowers yet.
- [obra/superpowers-chrome](https://github.com/obra/superpowers-chrome) - Chrome automation via DevTools Protocol, no deps.
- [tfriedel/claude-office-skills](https://github.com/tfriedel/claude-office-skills) - Office document skills (pptx/docx/xlsx/pdf) for the CLI. Predates Anthropic's official release; maintainer now points to the official repo.

## Authoring tools

- [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) - The official interactive skill for authoring and evaluating new skills. Start here.
- [skill-creator plugin](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/skill-creator) - Same thing packaged as a Claude Code plugin, with Q&A flow and benchmarking.
- [agentskills/skills-ref](https://github.com/agentskills/agentskills/tree/main/skills-ref) - Validator and prompt-XML generator for SKILL.md files.
- [FrancyJGLisboa/agent-skill-creator](https://github.com/FrancyJGLisboa/agent-skill-creator) - Converts plain-English workflows into validated skills. Installs to 14+ tools.
- [alirezarezvani/claude-code-skill-factory](https://github.com/alirezarezvani/claude-code-skill-factory) - Generates skills, agents, slash commands, and prompts in bulk.

## Reading & docs

- [Claude Code skills docs](https://code.claude.com/docs/en/skills) - The canonical reference: creating, storing, invoking, scoping.
- [Agent Skills overview (platform)](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview) - How skills work across the API, Claude.ai, and Claude Code. Read this to understand progressive disclosure.
- [Equipping agents for the real world with Agent Skills](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) - Anthropic's launch post, Oct 2025.
- [Introduction to Claude Skills - Cookbook notebook](https://platform.claude.com/cookbook/skills-notebooks-01-skills-introduction) - Runnable walkthrough.
- [The Complete Guide to Building Skills for Claude](https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf) - 33-page PDF, official.
- [Claude Skills are awesome, maybe a bigger deal than MCP](https://simonw.substack.com/p/claude-skills-are-awesome-maybe-a) - Simon Willison's take. The reason a lot of people paid attention in the first place.
- [Claude Skills - Simon Willison's notes](https://simonwillison.net/2025/Oct/10/claude-skills/) - His original writeup with the `/mnt/skills` extraction.
- [Superpowers: How I'm using coding agents in October 2025](https://blog.fsck.com/2025/10/09/superpowers/) - Jesse Vincent introducing the brainstorm-plan-implement workflow.
- [Why Everyone Should Try Claude Skills](https://nicknisi.com/posts/claude-skills/) - Nick Nisi, practical walkthrough with three example skills.
- [agentskills.io](https://agentskills.io) - Spec, client-implementation guide, adoption list.

## Related

Adjacent ecosystems you probably want alongside skills.

- [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) - Reference MCP servers.
- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - The canonical MCP servers list.
- [punkpeye/awesome-mcp-clients](https://github.com/punkpeye/awesome-mcp-clients) - MCP clients.
- [punkpeye/awesome-mcp-devtools](https://github.com/punkpeye/awesome-mcp-devtools) - SDKs, testing, and developer tooling for MCP.

## Use this list as a skill

This repo ships a small companion skill at [`skills/browse-awesome-skills`](skills/browse-awesome-skills/SKILL.md). It lets Claude search this list for you - ask for "a skill that does X" or "which collection should I install" and Claude will suggest entries from the sections above.

Install it into Claude Code (user scope):

```bash
mkdir -p ~/.claude/skills/browse-awesome-skills
curl -o ~/.claude/skills/browse-awesome-skills/SKILL.md \
  https://raw.githubusercontent.com/horiastanxd/awesome-claude-skills/main/skills/browse-awesome-skills/SKILL.md
```

Then in a Claude session, try: *"find me a skill for generating PowerPoint decks"* or *"which awesome-skills collection is worth installing?"*.

## Contributing

PRs welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the format. Short version: one line per entry, real link, no affiliate/referral URLs, and the skill has to actually work.
