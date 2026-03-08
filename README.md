# gtm-skills

GTM, GEO & SEO skills for Claude Code. Launch smarter. Rank in AI search. Optimize every page.

## What's inside

Three skill sets, 11 slash commands:

### GTM (Go-To-Market)

| Command | What it does |
|---------|-------------|
| `/gtm:positioning` | ICP definition, value prop canvas, competitive positioning |
| `/gtm:channels` | Channel-market fit matrix + 30-day action plans |
| `/gtm:pricing` | Value-based pricing analysis + competitive benchmarking |
| `/gtm:launch` | Pre-launch checklist (product, marketing, tech, legal) |
| `/gtm:metrics` | North star + KPI framework + measurement plan |

### GEO (Generative Engine Optimization)

| Command | What it does |
|---------|-------------|
| `/geo:score` | Score content for AI citability (0-100) |
| `/geo:optimize` | Rewrite content for ChatGPT, Perplexity, AI Overviews |
| `/geo:audit` | Audit a full site's GEO readiness |

### SEO

| Command | What it does |
|---------|-------------|
| `/seo:page` | Single-page SEO audit with scoring (0-100) |
| `/seo:schema` | Generate or validate Schema.org JSON-LD |
| `/seo:hreflang` | Validate hreflang for multilingual sites |

## Install

```bash
npx skills add ORBWEVA/gtm-skills
```

Or manually copy:
- `skills/` -> `~/.claude/skills/`
- `commands/` -> `~/.claude/commands/`

## Example output

### `/gtm:positioning` on a SaaS product

```
ICP PROFILE
============
Role/Title:      Solo founder, technical background
Company size:    Pre-revenue to $10K MRR
Pain trigger:    Built the product, stuck at 0 customers
Current solution:Generic marketing advice, Twitter threads
Budget authority:Full (it's their money)

POSITIONING STATEMENT
For solo founders who've built a product but can't get their
first 100 customers, LaunchKit is a GTM automation platform
that sequences outreach across proven channels. Unlike generic
marketing tools, we're purpose-built for pre-PMF SaaS with
templates that have driven 200+ successful launches.
```

### `/geo:score` on a blog post

```
GEO CITATION-READINESS SCORE
==============================
Structure:       18/25
Authority:       12/25
Extractability:  15/25
Technical:       20/25
-------------------------------
TOTAL:           65/100 (Good — specific optimizations needed)

TOP FIX: First paragraph is 4 sentences of preamble before
answering the question. Move the definition to sentence 1
to increase extractability by ~10 points.
```

### `/seo:page` on a landing page

```
SEO PAGE AUDIT
===============
Content:         22/30
Structure:       18/20
Technical:       15/25
Multilingual:    15/15 (N/A — single language)
Authority:        7/10
-------------------------------
TOTAL:           77/100 (Good)

PRIORITY FIX: No Schema markup detected. Add Article schema
with headline, author, datePublished, and inLanguage fields.
Estimated impact: +5-8 points.
```

## How the skills connect

```
/gtm:positioning  -->  /gtm:channels  -->  /gtm:pricing
       |                                        |
       v                                        v
/gtm:metrics  <--  /gtm:launch  <--  /seo:page + /geo:score
```

1. Start with positioning (who are you for?)
2. Pick channels (where will you reach them?)
3. Set pricing (what will you charge?)
4. Define metrics (how will you know it's working?)
5. Run the launch checklist (is everything ready?)
6. Audit your pages with SEO + GEO before going live

## CJK-aware

All SEO skills adjust automatically for CJK (Chinese, Japanese, Korean):
- Title limits: 30-35 chars (vs 50-60 for English)
- Description limits: 70-80 chars (vs 150-160 for English)
- Language codes: `ja` not `jp`, `ko` not `kr`
- Platform coverage: Google + Yahoo! Japan + Naver

## Security

Zero executable code. Pure markdown — structured prompts that guide Claude's thinking. No scripts, no dependencies, no API calls, no shell commands.

```
skills/gtm-launch/SKILL.md     # GTM methodology
skills/geo/SKILL.md            # GEO scoring + optimization
skills/seo-audit/SKILL.md      # SEO auditing + schema + hreflang
commands/gtm/*.md              # 6 GTM slash commands
commands/geo/*.md              # 4 GEO slash commands
commands/seo/*.md              # 4 SEO slash commands
package.json                   # metadata only
```

## License

MIT
