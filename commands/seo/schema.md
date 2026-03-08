---
name: seo schema
description: Generate or validate Schema.org structured data in JSON-LD format
---

Run the Schema Generation/Validation from `~/.claude/skills/seo-toolkit/SKILL.md`.

**If generating schema:**
1. Read the page content (URL, file, or description)
2. Determine the best schema type(s) from the supported types table
3. Generate complete JSON-LD with all required and recommended fields
4. Set `inLanguage` correctly (ja, en, ko — NOT jp, kr)
5. Include implementation instructions (where to place the script tag)

**If validating existing schema:**
1. Extract existing schema from the page
2. Run all 7 validation checks from the skill
3. Report issues with specific fixes
4. Generate corrected schema if errors found

Always output a complete, copy-paste-ready JSON-LD block wrapped in `<script type="application/ld+json">` tags.
