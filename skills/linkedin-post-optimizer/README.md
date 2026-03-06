# LinkedIn Post Optimizer

Transform raw ideas into LinkedIn posts that sound like **you**, not like AI.

## What It Does

```
Your raw idea → Structured post in YOUR voice
```

**Input:** Messy notes, bullet points, stream of consciousness

**Output:** Clean post that sounds like you wrote it (because you did — we just organized it)

## Setup

1. Copy `profile-context.example.md` to `profile-context.md`
2. Fill in your details:
   - Number of connections/followers
   - Number of posts you've published
   - Your natural tone (formal/casual/technical)
   - Typical post length you're comfortable with

## Adapts to Your Level

| Profile Level | Connections | Recommended Length | Advice |
|--------------|-------------|-------------------|--------|
| Beginner | < 500 | 100-150 words | Simple, one point, build credibility |
| Intermediate | 500-1500 | 150-220 words | Can experiment with structure |
| Advanced | 1500+ | 200-280 words | Audience trusts your takes |

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
