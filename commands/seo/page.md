---
name: seo page
description: Full single-page SEO audit with scoring (0-100)
---

Run the SEO Page Audit from `~/.claude/skills/seo-toolkit/SKILL.md`.

1. Read the page — URL (fetch it), file path, or ask the user
2. Score across all 5 categories: Content (30), Structure (20), Technical (25), Multilingual (15), Authority (10)
3. For each sub-criterion, score 0-5 with specific evidence from the page
4. Calculate total score and interpretation
5. For every issue found, provide the exact fix:
   - Current value → Recommended value
   - Code snippet if applicable (e.g., corrected meta tag, schema block)
6. Deliver a priority action list ordered by impact

For multilingual pages, score the Multilingual section fully. For single-language pages, award 15/15 for Multilingual and note it as N/A.

Be concrete. "Improve your title" is useless. "Change title from 'Home' to 'GTM Strategy Template — Free Launch Checklist | LaunchKit' (currently 4 chars, target 50-60)" is useful.
