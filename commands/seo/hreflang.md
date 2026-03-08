---
name: seo hreflang
description: Validate hreflang tags for multilingual sites
---

Run the Hreflang Validation from `~/.claude/skills/seo-audit/SKILL.md`.

1. Read the page(s) — URL, file path, or sitemap
2. Extract all hreflang tags from the page(s)
3. Run every check from the Hreflang Audit:
   - Structural checks (all versions present, self-referencing, x-default, reciprocal)
   - Common mistakes (jp vs ja, kr vs ko, redirected URLs, relative URLs)
   - Implementation format consistency
4. For each error, show:
   - What's wrong (with the actual incorrect tag)
   - The corrected tag
5. If pages are missing hreflang entirely, generate the complete set
6. Check the CJK-specific rules if Japanese or Korean pages are involved

Output corrected hreflang tags as copy-paste-ready HTML.
