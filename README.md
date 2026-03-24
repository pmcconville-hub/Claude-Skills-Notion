# Claude Skills

A collection of custom skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — Anthropic's agentic coding tool. Each skill extends Claude's capabilities with specialized workflows, domain expertise, and automation patterns.

## What Are Claude Skills?

Claude Skills are reusable instruction sets (`.md` files) that give Claude Code specialized abilities — from orchestrating Notion AI to building multi-agent teams. Drop a skill into your `~/.claude/skills/` directory and Claude gains a new capability you can invoke by name.

For the full skill development framework, tooling, and builder infrastructure, see the **[Skill Ecosystem](https://github.com/mrtblount/skill-ecosystem)** repo.

## Repository Structure

```
claude-skills/
├── README.md
├── LICENSE
├── notion-ai-orchestrator/
│   ├── README.md
│   └── SKILL.md
├── prd-builder/
│   ├── README.md
│   ├── SKILL.md
│   ├── references/
│   │   └── prd-template.md
│   └── sub-skills/
│       ├── discovery/SKILL.md
│       ├── researcher/SKILL.md
│       ├── generator/SKILL.md
│       └── reviewer/SKILL.md
└── (more skills coming)
```

## Skills

| Skill | Description |
|-------|-------------|
| [prd-builder](./prd-builder/) | AI-native PRD builder — structured discovery interviews, market research, generation, and review. Produces comprehensive Product Requirements Documents for new or existing products. |
| [notion-ai-orchestrator](./notion-ai-orchestrator/) | Orchestrate Notion AI through the Claude Chrome Extension — create databases, search content, modify pages, and set up automations by delegating to Notion's built-in AI agent. |

## Usage

1. Clone this repo (or copy individual skill folders)
2. Place skill folders in `~/.claude/skills/`
3. Invoke skills by name in Claude Code (e.g., "use notion ai to create a database")

## Links

- [Skill Ecosystem](https://github.com/mrtblount/skill-ecosystem) — Framework, builder tools, and skill development infrastructure
- [tonyblount.com](https://tonyblount.com) — Portfolio
- [Four30.co](https://four30.co) — Consulting
- [LinkedIn](https://www.linkedin.com/in/williamblount/)

## License

MIT — see [LICENSE](./LICENSE)
