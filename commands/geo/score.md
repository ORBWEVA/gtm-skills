---
name: geo score
description: Score a page's content for AI citability (0-100)
---

Run the GEO Scoring rubric from `~/.claude/skills/geo/SKILL.md`.

1. Read the page content — either from a URL (fetch it), a file path, or ask the user for the page to score
2. Score the page across all 4 categories: Structure (25), Authority (25), Extractability (25), Technical (25)
3. For each sub-criterion, give a score 0-5 with a brief justification
4. Calculate the total GEO Citation-Readiness Score
5. Identify the weakest category and explain why
6. Provide a prioritized fix list: what to change first for maximum impact
7. Show the score interpretation (Excellent / Good / Needs work / Poor)

Be specific in feedback. "Add schema" is bad. "Add Article schema with inLanguage: 'en', datePublished, and author fields" is good.
