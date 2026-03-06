# Agent Skills

A collection of agent skills for AI coding agents. Skills are packaged instructions that extend agent capabilities.

Works with Claude Code, Antigravity, Cursor, Codex, Amp, Cline, and [35+ other agents](https://github.com/vercel-labs/skills#supported-agents).

## Installation

```bash
npx skills add Smolevich/agent-skills
```

The CLI auto-detects your installed agents and sets up skills for each one.

Install a specific skill:

```bash
npx skills add Smolevich/agent-skills --skill linkedin-post-optimizer
```

## Available Skills

### linkedin-post-optimizer

Transform raw ideas into authentic LinkedIn posts adapted to the user's profile level, voice, and audience. Includes AI slop detection, voice preservation, and engagement optimization.

**Features:**
- 10-step workflow: idea → stats → topic sharpening → writing → expert review → refinement
- Profile-aware (Beginner / Intermediate / Advanced)
- Anti-AI-slop: actively removes patterns that scream "ChatGPT wrote this"
- Multilingual: RU/EN with language-audience mismatch detection
- Built-in expert review and iterative refinement loop

[View skill →](skills/linkedin-post-optimizer/SKILL.md)

## Usage

Once installed, skills activate automatically when you ask your agent a relevant question.

**Claude Code:**
```bash
/linkedin-post-optimizer drafts/my-post.md
```

**Codex / Antigravity / Cursor / other agents:**
```
"Write a LinkedIn post about switching from Cursor to CLI-first AI workflow"
```

## Skill Structure

Each skill contains:
- `SKILL.md` — Instructions for the agent
- `references/` — Supporting documentation (optional)
- `evals/` — Test cases (optional)

## License

MIT
