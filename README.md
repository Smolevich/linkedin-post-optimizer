# LinkedIn Post Optimizer

An agent skill that helps you write LinkedIn posts that sound like **you**, not like AI.

Works with Claude Code, Antigravity, Cursor, Codex, Amp, Cline, and [35+ other agents](https://github.com/vercel-labs/skills#supported-agents).

[![skills.sh](https://img.shields.io/badge/skills.sh-linkedin--post--optimizer-blue)](https://skills.sh/Smolevich/linkedin-post-optimizer)

## Installation

```bash
npx skills add Smolevich/linkedin-post-optimizer
```

The CLI auto-detects your installed agents and sets up the skill for each one.

## Philosophy

This is NOT about writing "viral LinkedIn posts."

This is about:
- Taking your raw idea and structuring it clearly
- Preserving your actual voice and style
- Adapting to your profile level (beginner → advanced)
- **Removing AI slop** so your posts feel authentic

## Features

- **Adaptive**: Adjusts recommendations based on your audience size, post history, and engagement
- **Voice preservation**: Keeps your words, removes friction
- **Anti-AI-slop**: Actively removes patterns that scream "ChatGPT wrote this"
- **Profile-aware**: Different advice for beginners vs advanced profiles
- **Multilingual**: Supports RU/EN with language-audience mismatch detection

## What It Does

```
Your raw idea → Structured post in YOUR voice
```

**Input:** Messy notes, bullet points, stream of consciousness

**Output:** Clean post that sounds like you wrote it (because you did — we just organized it)

## Setup

1. Copy `profile-context.example.md` to `profile-context.md`
2. Fill in your details:
   - SSI score (or estimate)
   - Number of posts you've published
   - Your natural tone (formal/casual/technical)
   - Typical post length you're comfortable with

## Usage

Once installed, the skill activates automatically when you ask your agent to write or improve a LinkedIn post.

**Claude Code:**
```bash
# Via slash command
/linkedin-post-optimizer drafts/my-post.md

# Or just ask
# "Help me write a LinkedIn post about my AI tools setup"
```

**Codex / Antigravity / Cursor / other agents:**
```
# Just ask naturally — the skill triggers automatically
"Write a LinkedIn post about switching from Cursor to CLI-first AI workflow"
"Help me draft a post about my experience with AI agents"
```

## Structure (Universal)

Every post needs three parts:

1. **Hook** — What makes someone stop scrolling
2. **Body** — The actual insight/story/information
3. **Conclusion** — Takeaway or question

That's it. No complex formulas.

## Adapts to Your Level

| Profile Level | SSI | Recommended Length | Advice |
|--------------|-----|-------------------|--------|
| Beginner | < 25 | 100-150 words | Simple, one point, build credibility |
| Intermediate | 25-50 | 150-220 words | Can experiment with structure |
| Advanced | 50+ | 200-280 words | Audience trusts your takes |

## Anti-AI-Slop

The skill actively removes:

- "In today's fast-paced world..."
- "Let's dive in..."
- "Game-changer", "unlock", "leverage"
- Excessive emoji
- Perfect bullet point symmetry
- Overly smooth transitions

**The test:** Would you actually say this out loud?

## Example

**Your draft:**
```
spent whole weekend debugging auth bug, finally fixed it by reading the actual docs lol
```

**Bad output (AI slop):**
```
This weekend, I encountered a challenging authentication bug.
After extensive debugging, I discovered the solution was in
the documentation all along. Key lesson: always RTFM! 📚

#Engineering #Debugging #SoftwareDevelopment
```

**Good output (your voice):**
```
Spent the whole weekend on one auth bug.
The fix? Actually reading the docs.

Sometimes the answer is embarrassingly obvious.
```

## License

MIT
