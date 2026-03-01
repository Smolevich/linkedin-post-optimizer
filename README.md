# LinkedIn Post Optimizer

A Claude Code skill that helps you write LinkedIn posts that sound like **you**, not like AI.

## Philosophy

This is NOT about writing "viral LinkedIn posts."

This is about:
- Taking your raw idea and structuring it clearly
- Preserving your actual voice and style
- Adapting to your profile level (beginner → advanced)
- **Removing AI slop** so your posts feel authentic

## Features

- **Adaptive**: Adjusts recommendations based on your SSI, post history, and style
- **Voice preservation**: Keeps your words, removes friction
- **Anti-AI-slop**: Actively removes patterns that scream "ChatGPT wrote this"
- **Profile-aware**: Different advice for SSI 19 vs SSI 50

## What It Does

```
Your raw idea → Structured post in YOUR voice
```

**Input:** Messy notes, bullet points, stream of consciousness

**Output:** Clean post that sounds like you wrote it (because you did — we just organized it)

## Installation

```bash
# In your project root
mkdir -p .claude/skills
git clone https://github.com/Smolevich/linkedin-post-optimizer .claude/skills/linkedin-post-optimizer
```

## Setup

1. Copy `profile-context.example.md` to `profile-context.md`
2. Fill in your details:
   - SSI score (or estimate)
   - Number of posts you've published
   - Your natural tone (formal/casual/technical)
   - Typical post length you're comfortable with

## Usage

```bash
# Create a draft with your raw idea
echo "My messy thoughts about AI tools..." > drafts/my-post.md

# Run the optimizer
/linkedin-post-optimizer drafts/my-post.md
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

## Based On

Real data from 25+ posts with 28K+ total impressions. But your mileage will vary — that's why the skill adapts to YOUR profile, not copy-pastes a formula.

## License

MIT
