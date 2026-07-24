# Valency Agent Skills

Portable research-corpus workflows for AI coding agents that use the
[Valency MCP server](https://docs.valency.io/).

The repository follows the open Agent Skills layout expected by Vercel's
[`skills` CLI](https://vercel.com/docs/agent-resources/skills): each skill lives
at `skills/<skill-name>/SKILL.md` and declares a unique `name` and
`description` in YAML frontmatter.

## Install

Install the collection:

```bash
npx skills@latest add valency-oss/valency-skills
```

List the available skills without installing them:

```bash
npx skills@latest add valency-oss/valency-skills --list
```

Install one skill:

```bash
npx skills@latest add valency-oss/valency-skills --skill valency-profile
```

Add `-g` to install at user scope instead of into the current project. The CLI
will detect supported agents and prompt for the installation targets.

These skills require the Valency MCP server to be configured in the target
agent. They do not install or authenticate the MCP connection themselves.

## Included skills

| Skill | Purpose |
| --- | --- |
| `valency-profile` | Build a researcher's publication and collaboration profile |
| `valency-landscape` | Summarize a field, its growth, authors, and subdomains |
| `valency-similar` | Find papers semantically similar to a known paper |
| `valency-trends` | Analyze publication trends for topics or categories |
| `valency-network` | Map collaborators and research divergence |
| `valency-reading-list` | Curate reading by a researcher's intellectual threads |
| `valency-fresh-collaborators` | Find relevant researchers outside an existing network |
