---
name: seo-toolkit
description: Single-page SEO analysis and scoring. Use when user wants to audit a page for SEO, check meta tags, validate schema, review hreflang, or optimize on-page elements. Triggers on "SEO audit", "page SEO", "check my SEO", "meta tags", "schema markup", "hreflang", or /seo commands.
---

# SEO Audit Skill

Practical, actionable SEO analysis for individual pages. Score a page, generate schema markup, and validate multilingual hreflang implementations.

## Commands

| Command | What it does |
|---------|-------------|
| `/seo:page` | Full single-page SEO audit with scoring |
| `/seo:schema` | Generate or validate Schema.org structured data |
| `/seo:hreflang` | Validate hreflang tags for multilingual sites |
| `/seo:help` | Command reference |

---

## Page Audit (`/seo:page`)

**Goal:** Score a page's on-page SEO and identify specific fixes.

### Audit Rubric (100 points)

```
SEO PAGE AUDIT
===============

CONTENT (30 points)
  [ /5 ] Title tag: present, unique, includes target keyword
  [ /5 ] Title length: EN 50-60 chars | CJK 30-35 chars
  [ /5 ] H1: present, unique, matches search intent
  [ /5 ] Meta description: present, compelling, includes keyword
  [ /5 ] Meta description length: EN 150-160 chars | CJK 70-80 chars
  [ /5 ] First paragraph contains target keyword naturally

STRUCTURE (20 points)
  [ /5 ] Heading hierarchy is logical (H1 > H2 > H3, no skips)
  [ /5 ] URL slug is descriptive and keyword-relevant
  [ /5 ] Internal links to 2+ related pages
  [ /5 ] Images have descriptive alt text

TECHNICAL (25 points)
  [ /5 ] Schema markup present and valid (Article, Product, FAQ, etc.)
  [ /5 ] Open Graph tags present (og:title, og:description, og:image)
  [ /5 ] Canonical URL set correctly
  [ /5 ] Mobile viewport meta tag present
  [ /5 ] Page loads fast (LCP < 2.5s, CLS < 0.1, INP < 200ms)

MULTILINGUAL (15 points) — score 15/15 if single-language
  [ /5 ] hreflang tags present for all language versions
  [ /5 ] Self-referencing hreflang included
  [ /5 ] x-default set (typically to homepage or EN version)

AUTHORITY (10 points)
  [ /5 ] Content answers the search query directly
  [ /5 ] At least one unique data point or original insight

TOTAL: ___/100
```

### Score Interpretation

| Score | Rating | Action |
|-------|--------|--------|
| 85-100 | Excellent | Minor tweaks only. Focus on content freshness. |
| 70-84 | Good | Address specific gaps. Likely ranks but leaving value on table. |
| 50-69 | Needs work | Significant optimization needed. Multiple ranking signals missing. |
| 0-49 | Poor | Fundamental SEO elements missing. Likely invisible to search. |

### Output
Deliver: Score breakdown + specific issues with line-by-line fixes + priority action list.

---

## Schema Generation (`/seo:schema`)

**Goal:** Generate or validate Schema.org structured data in JSON-LD format.

### Supported Schema Types

| Type | When to use |
|------|------------|
| Article | Blog posts, news articles, guides |
| Product | Product pages, SaaS pricing pages |
| FAQ | FAQ pages, pages with Q&A sections |
| HowTo | Tutorial content, step-by-step guides |
| LocalBusiness | Business location pages |
| Organization | About pages, company pages |
| BreadcrumbList | Any page with breadcrumb navigation |
| WebSite | Homepage (with SearchAction for sitelinks search) |
| Person | Author pages, team member pages |
| Course | Online course/lesson pages |
| SoftwareApplication | App/tool pages |
| VideoObject | Pages with embedded video |

### Schema Output Format

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "Page title here",
  "description": "Meta description here",
  "inLanguage": "en",
  "author": {
    "@type": "Person",
    "name": "Author Name"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Company Name",
    "logo": {
      "@type": "ImageObject",
      "url": "https://example.com/logo.png"
    }
  },
  "datePublished": "2026-03-01",
  "dateModified": "2026-03-08",
  "mainEntityOfPage": {
    "@type": "WebPage",
    "@id": "https://example.com/page"
  }
}
```

### Schema Validation Checks

1. Required fields present for the schema type
2. `inLanguage` matches the page's actual language (ja, en, ko — NOT jp, kr)
3. URLs are absolute, not relative
4. Dates are in ISO 8601 format
5. No conflicting schema types on the same page
6. Nested entities (@type within @type) are valid
7. Images referenced in schema actually exist

### Output
Deliver: Complete JSON-LD schema block + validation results + implementation instructions.

---

## Hreflang Validation (`/seo:hreflang`)

**Goal:** Validate hreflang implementation for multilingual sites.

### Validation Checks

```
HREFLANG AUDIT
===============

STRUCTURAL CHECKS
  [ ] Every page has hreflang tags for ALL language versions
  [ ] Self-referencing hreflang present on every page
  [ ] x-default tag present (points to canonical/default version)
  [ ] Reciprocal links: if Page A links to Page B, Page B links back to A
  [ ] hreflang values use correct ISO 639-1 codes
  [ ] Region codes (if used) follow ISO 3166-1 Alpha-2

COMMON MISTAKES
  [ ] NOT using "jp" instead of "ja" for Japanese
  [ ] NOT using "kr" instead of "ko" for Korean
  [ ] NOT mixing language-only and language-region codes inconsistently
  [ ] NOT pointing hreflang to redirected URLs
  [ ] NOT using relative URLs in hreflang tags
  [ ] NOT missing pages (every language version of every page must be included)

IMPLEMENTATION FORMAT
  [ ] Consistent method: <link> tags in <head> OR HTTP headers OR sitemap
  [ ] Not mixing multiple implementation methods
```

### Correct hreflang Format

```html
<!-- On English page: example.com/about -->
<link rel="alternate" hreflang="en" href="https://example.com/about" />
<link rel="alternate" hreflang="ja" href="https://example.com/ja/about" />
<link rel="alternate" hreflang="ko" href="https://example.com/ko/about" />
<link rel="alternate" hreflang="x-default" href="https://example.com/about" />
```

### Language Code Reference

| Language | Correct | WRONG |
|----------|---------|-------|
| Japanese | `ja` | `jp` |
| Korean | `ko` | `kr` |
| English | `en` | `eng` |
| Chinese (Simplified) | `zh-Hans` or `zh-CN` | `cn` |
| Chinese (Traditional) | `zh-Hant` or `zh-TW` | `tw` |
| Portuguese (Brazil) | `pt-BR` | `br` |
| English (Australia) | `en-AU` | `au` |

### CJK-Specific SEO Rules

When auditing CJK (Chinese, Japanese, Korean) pages:

1. **Title length:** 30-35 characters (CJK characters display wider)
2. **Meta description:** 70-80 characters
3. **HTML `lang` attribute** must match content language
4. **No mixed-language content** on a single page (except brand names)
5. **Keywords are NOT translations** — research natively per language
6. **Platform requirements:**
   - Japan: Google + Yahoo! Japan (register with Yahoo! Japan Site Explorer)
   - Korea: Naver (~58% market share) + Google (register with Naver Search Advisor)

### Output
Deliver: Hreflang audit results + specific errors + corrected hreflang tags + missing page pairs.

---

## Quick Reference: SEO Essentials

### Title Tag Formula
```
[Primary Keyword] — [Benefit/Modifier] | [Brand]
```
Example: `GTM Strategy Template — Free Launch Checklist | LaunchKit`

### Meta Description Formula
```
[What the page covers]. [Key benefit]. [CTA or unique value prop].
```
Example: `A step-by-step go-to-market strategy template covering positioning, channels, pricing, and launch execution. Used by 500+ SaaS founders. Download free.`

### URL Slug Rules
- Lowercase, hyphen-separated
- Include target keyword
- No dates, IDs, or parameters in informational content URLs
- Keep under 60 characters

### Internal Linking Rules
- Every page links to 2+ related pages
- Use descriptive anchor text (not "click here")
- Link from high-authority pages to pages you want to rank
- Keep important pages within 3 clicks from homepage

---

## Principles

1. **Search intent first.** Match the page type to what the searcher actually wants (information, comparison, purchase, navigation).
2. **One page, one keyword cluster.** Don't try to rank a single page for unrelated keywords.
3. **Technical SEO is table stakes.** Schema, speed, mobile — these aren't competitive advantages, they're minimum requirements.
4. **Multilingual means multi-market.** Each language version needs native keyword research, not translations.
5. **Measure what ranks.** Track keyword positions and organic traffic, not vanity metrics.
