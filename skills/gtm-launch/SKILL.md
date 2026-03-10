---
name: gtm-launch
description: Go-to-market launch framework for products and features. Use when user wants to plan a launch, define positioning, evaluate channels, set pricing strategy, or build a KPI framework. Triggers on "go to market", "GTM", "launch plan", "positioning", "channel strategy", "pricing strategy", or /gtm commands.
---

# Go-To-Market Skill

A structured framework for taking products and features to market. Moves you from "we built something" to "here's who it's for, how we'll reach them, how we'll price it, and how we'll know it's working."

## Commands

| Command | What it does |
|---------|-------------|
| `/gtm:launch` | Full pre-launch checklist across product, marketing, technical, and legal |
| `/gtm:positioning` | ICP definition + value prop canvas + competitive positioning statement |
| `/gtm:channels` | Channel-market fit matrix with prioritization |
| `/gtm:pricing` | Pricing strategy analysis (value-based, competitive, penetration) |
| `/gtm:metrics` | North star metric + supporting KPIs + measurement plan |
| `/gtm:outreach` | Cold email + LinkedIn sequences with personalization scoring |
| `/gtm:landing` | Landing page CRO audit with scoring and copy fixes |
| `/gtm:growth` | PLG growth loops, referrals, activation, free tools |
| `/gtm:help` | Command reference |

---

## Stage 1: Positioning (`/gtm:positioning`)

**Goal:** Define exactly who you're for, what you do for them, and why you over alternatives.

### Process

1. **Define your ICP (Ideal Customer Profile).** Be ruthlessly specific:

```
ICP PROFILE
============
Role/Title:      [Who buys or champions this?]
Company size:    [Revenue range, employee count, stage]
Industry:        [Vertical or horizontal?]
Pain trigger:    [What event makes them start looking?]
Current solution:[What are they using today?]
Budget authority:[Do they control budget or need approval?]
Success metric:  [What do they measure themselves on?]
```

2. **Build a Value Proposition Canvas:**

```
VALUE PROP CANVAS
==================
CUSTOMER SIDE                    PRODUCT SIDE
─────────────                    ────────────
Jobs to be done:                 Features:
  1. [Functional job]              1. [Maps to job 1]
  2. [Social job]                  2. [Maps to job 2]
  3. [Emotional job]               3. [Maps to job 3]

Pains:                           Pain relievers:
  1. [Current frustration]         1. [How you fix it]
  2. [Risk they fear]              2. [How you reduce it]

Gains:                           Gain creators:
  1. [Desired outcome]             1. [How you enable it]
  2. [Unexpected delight]          2. [How you deliver it]
```

3. **Write a Positioning Statement:**

```
For [ICP] who [pain trigger],
[Product] is a [category]
that [key benefit].
Unlike [primary alternative],
we [key differentiator].
```

**Good example:**
> For solo founders launching SaaS products who struggle to reach their first 100 customers, LaunchKit is a GTM automation platform that sequences your outreach across channels. Unlike generic marketing tools, we're built specifically for pre-PMF products with templates proven at early stage.

**Bad example:**
> For everyone who wants to grow, we're the best platform. (No ICP, no differentiator, no category)

4. **Competitive Positioning Map.** Plot on two axes that matter to your ICP:

```
                    [Axis 2: e.g., Ease of use]
                         HIGH
                          |
              Competitor A|    YOUR PRODUCT
                          |         *
          ────────────────┼─────────────────
          LOW             |              HIGH
              Competitor B|    Competitor C
                          |
                         LOW
                    [Axis 1: e.g., Feature depth]
```

Choose axes where you win. If you can't find two axes where you're top-right, revisit your differentiation.

### Output
Deliver: ICP profile + Value Prop Canvas + Positioning Statement + Competitive Position Map.

---

## Stage 2: Channels (`/gtm:channels`)

**Goal:** Identify where your ICP hangs out and how to reach them cost-effectively.

### Process

1. **List candidate channels.** Consider all of these:

| Category | Channels |
|----------|----------|
| Content | Blog/SEO, YouTube, podcast, newsletter, social media |
| Paid | Google Ads, Meta Ads, LinkedIn Ads, sponsorships |
| Outbound | Cold email, LinkedIn DMs, partnerships, events |
| Product-led | Freemium, referral program, marketplace listing, integrations |
| Community | Reddit, Discord, Slack communities, forums, Twitter/X |
| AI/GEO | AI search optimization, LLM mentions, ChatGPT plugins |

2. **Score each channel with the Channel-Market Fit Matrix:**

```
CHANNEL-MARKET FIT MATRIX
===========================
Channel          | ICP Present? | CAC Est. | Time to Result | Scalable? | SCORE
─────────────────┼──────────────┼──────────┼────────────────┼───────────┼──────
LinkedIn content |     5/5      |   Low    |   2-4 weeks    |    3/5    |
SEO/Blog         |     4/5      |   Low    |   3-6 months   |    5/5    |
Google Ads       |     4/5      |   High   |   1 week       |    4/5    |
Cold email       |     3/5      |   Med    |   1-2 weeks    |    3/5    |
...              |              |          |                |           |

Scoring: ICP Present (1-5) x Scalability (1-5) / CAC rank = weighted score
```

3. **Select 2-3 primary channels.** More than 3 = diluted effort pre-PMF.

4. **For each selected channel, define:**
   - First 30-day action plan
   - Content/creative needs
   - Tools required
   - Expected cost (time + money)
   - Leading indicators to track

### Output
Deliver: Channel-Market Fit Matrix + 2-3 selected channels + 30-day action plan per channel.

---

## Stage 3: Pricing (`/gtm:pricing`)

**Goal:** Set a pricing strategy grounded in value, not guesswork.

### Process

1. **Identify pricing model options:**

| Model | Best for | Risk |
|-------|----------|------|
| Flat rate | Simple products, clear value | Leaves money on the table at scale |
| Tiered | Multiple ICPs or usage levels | Complexity, choice paralysis |
| Usage-based | API, infrastructure, variable consumption | Revenue unpredictability |
| Per-seat | Collaboration tools, team products | Discourages adoption |
| Freemium | Product-led growth, network effects | Conversion rate pressure |
| Reverse trial | High-value products, complex onboarding | Churn spike at trial end |

2. **Run the Value-Based Pricing Analysis:**

```
VALUE-BASED PRICING
====================
1. What does the customer pay today?        $___/mo (current solution)
2. What does inaction cost them?            $___/mo (cost of problem)
3. What's the ROI of solving this?          ___x return
4. What's the switching cost?               $___  (migration + learning)
5. Willingness to pay (estimate):           $___/mo
6. Your cost to serve:                      $___/mo
7. Target margin:                           ___%

PRICE RANGE: $[cost to serve + margin] — $[willingness to pay]
RECOMMENDED: $[sweet spot with justification]
```

3. **Competitive Price Benchmarking:**

```
COMPETITIVE PRICING
====================
Competitor      | Price    | What's included        | Positioning
────────────────┼──────────┼────────────────────────┼──────────────
Competitor A    | $49/mo   | Feature set X          | Premium
Competitor B    | $19/mo   | Feature set Y          | Budget
Free alt        | $0       | Limited Z              | DIY
YOUR PRODUCT    | $__/mo   | [Your feature set]     | [Your angle]
```

4. **Pricing page structure recommendation:**
   - Number of tiers (recommend 3 max)
   - Feature differentiation between tiers
   - Anchor tier (which one you want people to pick)
   - Free tier / trial strategy

### Output
Deliver: Model recommendation + Value-Based Pricing analysis + Competitive benchmarking + Tier structure.

---

## Stage 4: Launch Checklist (`/gtm:launch`)

**Goal:** Ensure nothing falls through the cracks on launch day.

### Pre-Launch Checklist

```
GTM LAUNCH CHECKLIST
=====================

PRODUCT READINESS
  [ ] Core feature complete and tested
  [ ] Onboarding flow tested with 3+ real users
  [ ] Error states and edge cases handled
  [ ] Performance benchmarks met (LCP < 2.5s, etc.)
  [ ] Mobile experience verified
  [ ] Billing/payment flow tested end-to-end
  [ ] Support documentation written (FAQ, help docs)
  [ ] Feedback collection mechanism in place

MARKETING READINESS
  [ ] Positioning statement finalized
  [ ] Landing page live with clear CTA
  [ ] SEO: Title, meta description, schema markup, OG tags
  [ ] GEO: Content structured for AI citability (see /geo:score)
  [ ] Social proof elements (testimonials, logos, metrics)
  [ ] Launch announcement drafted (blog, social, email)
  [ ] Content calendar for first 30 days post-launch
  [ ] PR/outreach list prepared (if applicable)

TECHNICAL READINESS
  [ ] Analytics installed (events, funnels, attribution)
  [ ] Error monitoring active (Sentry, LogRocket, etc.)
  [ ] Uptime monitoring configured
  [ ] DNS/SSL/CDN verified
  [ ] Backup and recovery plan tested
  [ ] Rate limiting and abuse prevention in place
  [ ] GDPR/privacy compliance (cookie consent, privacy policy, DPA)

OPERATIONS READINESS
  [ ] Support channels established (email, chat, etc.)
  [ ] Escalation path defined
  [ ] SLA commitments documented
  [ ] Team roles for launch day assigned
  [ ] Rollback plan documented (if something breaks)

LEGAL READINESS
  [ ] Terms of Service published
  [ ] Privacy Policy published
  [ ] Cookie policy (if applicable)
  [ ] Trademark/IP check completed
  [ ] Data processing agreements ready (if B2B)
```

### Launch Day Run Sheet

```
LAUNCH DAY RUN SHEET
=====================
T-2h:  Final smoke test (core flow, payments, signup)
T-1h:  Team standup — confirm everyone's ready
T-0:   Flip the switch (DNS, feature flag, or publish)
T+5m:  Verify: site up, signup works, payment works
T+15m: Post launch announcement (social, email, communities)
T+1h:  Check: first signups, error rates, support queue
T+4h:  Debrief — what's working, what needs immediate attention
T+24h: Day 1 metrics review vs. targets
T+7d:  Week 1 retrospective
```

### Output
Deliver: Completed checklist (checked/unchecked per item) + Launch day run sheet + Risk assessment.

---

## Stage 5: Metrics (`/gtm:metrics`)

**Goal:** Define what success looks like with measurable KPIs.

### Process

1. **Define your North Star Metric.**

The one number that best captures the value you deliver to customers:

```
NORTH STAR METRIC
==================
Metric:     [e.g., "Weekly active conversations" or "Revenue per user"]
Why:        [Why this captures customer value, not just business value]
Target:     [Specific number + timeframe]
Measured:   [How/where — analytics tool, database query, etc.]
```

2. **Build your KPI Tree:**

```
                    NORTH STAR
                   /    |     \
            Acquisition  Activation  Revenue
            /    \        /    \       /    \
        Traffic  Conv%  Onboard  Aha!  ARPU  Churn
```

3. **KPI Framework (AARRR adapted):**

```
KPI FRAMEWORK
==============
Stage        | Metric              | Target  | Tool      | Frequency
─────────────┼─────────────────────┼─────────┼───────────┼──────────
Awareness    | Site visitors       |         | Analytics | Weekly
Acquisition  | Signup rate         |         | Analytics | Weekly
Activation   | Completed onboarding|        | Product   | Weekly
Revenue      | MRR / ARPU          |         | Stripe    | Weekly
Retention    | 30-day retention    |         | Product   | Monthly
Referral     | Referral rate       |         | Product   | Monthly
```

4. **Anti-Metrics (what NOT to optimize for):**

List 2-3 vanity metrics that feel good but don't matter:
- e.g., "Total signups" (without activation = meaningless)
- e.g., "Page views" (without conversion context)
- e.g., "Social followers" (without engagement)

5. **Measurement Plan:**

For each KPI, specify:
- Event name / tracking implementation
- Where it's tracked (GA4, Mixpanel, Stripe, custom)
- Dashboard location
- Alert thresholds (when to worry)
- Review cadence

### Output
Deliver: North Star definition + KPI tree + KPI framework table + Anti-metrics + Measurement plan.

---

## Stage 6: Outreach (`/gtm:outreach`)

**Goal:** Get your first conversations with potential customers through cold email and LinkedIn.

### Sales Triggers

Before writing a single message, identify what's happening at the target company that makes your product relevant *right now*:

| Category | Trigger examples |
|----------|-----------------|
| Hiring | Posting roles your product replaces/supports, new VP/Head of X |
| Funding | Raised a round, acquired a company, IPO prep |
| Technology | Adopted a tool you integrate with, migrating platforms |
| Content | Published a blog post about the problem you solve, spoke at a conference |
| Company event | Launched a new product, expanded to new market, hit a milestone |
| Performance | Revenue growth/decline visible in public data, layoffs, restructuring |

### Messaging Tiers

Match your tone and angle to who you're writing to:

```
ABOVE THE LINE (VP / C-Suite / Founder)
  - Lead with business outcome, not feature
  - Reference strategic decisions they've made
  - Short (3-5 sentences max)
  - Ask for a conversation, not a demo

BELOW THE LINE (Manager / IC / Practitioner)
  - Lead with the workflow pain you eliminate
  - Reference the tool/process they use today
  - Can be slightly longer (show you understand their day)
  - Offer something useful (template, benchmark, insight)
```

### SPARK Email Framework

Write every cold email using SPARK:

```
SPARK FRAMEWORK
================
S — Subject line:    Pattern-interrupt or curiosity gap (no clickbait)
P — Personalized:    First sentence references THEIR specific situation
A — Agitate:         Name the pain or cost of the status quo (1 sentence)
R — Relevant value:  How you solve it, with a specific proof point
K — Kick-off CTA:    One clear, low-friction ask
```

**Good example (BTL):**
```
Subject: Replacing your manual QA checklist

Hi [Name], saw your team shipped 3 releases last week — impressive
pace for a team of 6.

Quick question: how much time is your QA lead spending on regression
checklists between releases?

We built [Product] to auto-generate regression suites from PR diffs.
[Similar Company] cut their QA cycle from 4 hours to 20 minutes.

Worth a 15-min look? I can show you on your own repo.
```

**Bad example:**
```
Subject: Exciting opportunity!

Hi, I hope this email finds you well! I wanted to reach out because
our revolutionary AI-powered platform is transforming how companies
approach quality assurance. We have many features including...
(NO personalization, NO trigger, NO specific value, NO clear CTA)
```

### 3-Touch Email Sequence

```
OUTREACH SEQUENCE
==================
Touch 1 (Day 0):   SPARK email — trigger + value + CTA
Touch 2 (Day 3):   Value-add follow-up — share a relevant insight,
                    benchmark, or case study (NOT "just checking in")
Touch 3 (Day 7):   Breakup email — acknowledge they're busy,
                    leave the door open with one specific reason
                    to reply ("If [pain] ever becomes a priority...")
```

### LinkedIn Sequence

```
LINKEDIN SEQUENCE
==================
Connection request: 1 sentence max. Reference shared context
                    (mutual connection, same industry, their content).
                    NO pitch in the connection request.

Follow-up (Day 2):  After they accept — lead with value, not ask.
                     Share an insight relevant to their role.
                     End with a soft question, not a meeting request.
```

### Personalization Hierarchy

Score every message before sending:

```
PERSONALIZATION LEVELS
=======================
Level 0: No personalization (spray and pray)           — NEVER send
Level 1: Name + company only                           — NEVER send
Level 2: Industry or role-based                        — Minimum for low-ACV
Level 3: Company-specific (trigger, news, tech stack)  — Minimum for mid-ACV
Level 4: Person-specific (content they wrote, talks)   — Ideal for high-ACV
Level 5: Behavioral (visited your site, used free tool) — Best conversion rate
```

**Rule:** Level 3+ for any B2B outreach. Below that, you're spamming.

### Output
Deliver: Sales triggers identified + 3-touch email sequence + LinkedIn sequence + personalization score per message + send cadence timeline.

---

## Stage 7: Landing Page CRO (`/gtm:landing`)

**Goal:** Audit and optimize your landing page to convert visitors into signups or customers.

### The 8-Second Test

A first-time visitor decides in ~8 seconds whether to stay or bounce. In that window they need to understand:
1. **What** this product does
2. **Who** it's for
3. **Why** they should care

If your hero section doesn't answer all three, nothing below the fold matters.

### CRO Scoring Rubric (7 dimensions, 10 points each = 70 total)

```
LANDING PAGE CRO SCORE
========================

VALUE PROP CLARITY (0-10)
  Is it immediately obvious what this product does and who it's for?
  10 = Crystal clear in one sentence
  5  = Takes 2-3 sentences to understand
  0  = Visitor can't tell what this is

HEADLINE EFFECTIVENESS (0-10)
  Does the headline communicate the primary benefit (not a feature)?
  10 = Benefit-driven, specific, compelling
  5  = Descriptive but generic
  0  = Clever/vague ("Reimagine your workflow")

CTA HIERARCHY (0-10)
  Is there one clear primary action? Is it visible above the fold?
  10 = Single clear CTA, high contrast, benefit-labeled
  5  = Multiple competing CTAs or generic label ("Submit")
  0  = CTA buried or missing

VISUAL HIERARCHY (0-10)
  Does the eye flow naturally: headline → subhead → CTA → proof?
  10 = Clean flow, strong contrast, no distractions
  5  = Cluttered but navigable
  0  = Wall of text, no visual structure

TRUST SIGNALS (0-10)
  Are there credibility elements near the CTA?
  10 = Specific testimonials + logos + metrics
  5  = Generic testimonials or logos only
  0  = No social proof

OBJECTION HANDLING (0-10)
  Does the page address the top 3 reasons someone wouldn't buy?
  10 = Proactively addresses objections with evidence
  5  = Partially addresses 1-2 objections
  0  = Ignores objections entirely

FRICTION POINTS (0-10)
  How many unnecessary steps/fields/decisions before conversion?
  10 = Minimal friction (email-only signup, no CC required)
  5  = Some friction (long form, CC required, multi-step)
  0  = High friction (requires phone call, complex setup)

TOTAL: ___/70
```

### Score Interpretation

| Score | Rating | Action |
|-------|--------|--------|
| 56-70 | Strong | A/B test refinements |
| 42-55 | Good | Fix weakest 2 dimensions |
| 28-41 | Needs work | Significant rewrite needed |
| 0-27 | Poor | Start over with positioning-first approach |

### Objection/Counter-Objection Table

Build this for every product:

```
OBJECTION MAP
==============
Objection                    | Counter-objection              | Where to place it
─────────────────────────────┼────────────────────────────────┼──────────────────
"Too expensive"              | ROI calculator or comparison   | Near pricing
"Looks complex"              | "Set up in 5 minutes" + video  | Below hero
"Will it work for my case?"  | Specific use case examples     | Mid-page
"Can I trust this company?"  | Logos, testimonials, metrics   | Near CTA
"What if I don't like it?"   | Free trial / money-back        | Near CTA
```

### Copy Fixes (Before/After Pattern)

For each weak dimension, provide:

```
DIMENSION: [e.g., Headline Effectiveness — 4/10]

BEFORE: "The Modern Platform for Teams"
  Problem: Generic, no benefit, could be anything

AFTER:  "Ship 3x faster without breaking production"
  Why:    Specific benefit + addresses a fear + implies speed

EXPECTED IMPACT: +2-3 points on this dimension
```

### A/B Test Hypotheses

Suggest 2-3 tests using this format:

```
HYPOTHESIS: If we [change], then [metric] will [improve] because [reason]
VARIANT:    [Specific change to test]
METRIC:     [Primary metric to measure]
IMPACT:     HIGH / MED / LOW
EFFORT:     LOW / MED / HIGH
```

### Output
Deliver: CRO score (7 dimensions) + specific fixes with before/after copy + objection map + A/B test hypotheses + #1 quick win.

---

## Stage 8: Growth (`/gtm:growth`)

**Goal:** Design repeatable growth loops that compound over time — not one-shot campaigns.

### Growth Model Assessment

First, identify which model the product uses:

```
GROWTH MODEL
=============
[ ] Self-serve / PLG    — User signs up, gets value, upgrades
[ ] Sales-led           — Outbound/inbound → demo → close
[ ] Hybrid              — Self-serve for small, sales for enterprise
[ ] Community-led       — Community drives awareness → product adoption
[ ] Content-led         — Content drives organic traffic → signups
```

### Growth Loops

Campaigns are linear (spend money → get result → stop → result stops). Loops compound:

```
GROWTH LOOP TYPES
==================

VIRAL LOOP
  User gets value → shares with peer → peer signs up → peer gets value → shares
  Best for: Collaboration tools, social products, anything with network effects
  Key metric: Viral coefficient (K-factor > 1 = exponential growth)

CONTENT LOOP
  Create content → ranks in search/AI → drives traffic → some convert → users
  generate data/usage → create more content from it
  Best for: SaaS with public use cases, marketplaces, data products
  Key metric: Organic traffic → signup rate

PRODUCT-LED SALES LOOP
  User signs up free → gets value → team adopts → usage hits threshold →
  sales reaches out → enterprise deal
  Best for: B2B tools with individual + team use cases
  Key metric: PQA (Product-Qualified Accounts) → enterprise conversion rate
```

### Activation Design

The most important growth lever is getting new users to the "aha moment" fast:

```
ACTIVATION FRAMEWORK
=====================
1. DEFINE THE AHA MOMENT
   What action, when completed, makes a user unlikely to churn?
   Examples:
   - Slack: Sent 2,000 messages as a team
   - Dropbox: Put 1 file in 1 folder on 1 device
   - Zoom: Completed first call

2. MAP THE CURRENT FLOW
   Signup → [step] → [step] → [step] → Aha moment
   Time to aha: ___ minutes/hours/days
   Drop-off points: Where do users quit?

3. OPTIMIZE TIME-TO-VALUE
   Remove steps between signup and aha moment
   Can you deliver value BEFORE signup? (reverse trial, free tool)
   Can you pre-fill, auto-detect, or skip configuration?

4. RECOVER STALLED USERS
   Trigger: User signed up but didn't reach aha within [X time]
   Action: Email/notification with the ONE next step
   Tone: Helpful, not nagging
```

### Referral Loop Design

```
REFERRAL LOOP
==============
TRIGGER MOMENT:  When does the user feel most delighted?
                 (After first success, after a milestone, after sharing a result)

SHARE MECHANISM: How do they invite others?
                 [ ] In-product invite (best)
                 [ ] Share a result/output (good — shows value)
                 [ ] Referral link (ok — no inherent value)
                 [ ] Word of mouth only (worst — no leverage)

INCENTIVE MODEL:
  Single-sided:  Only referrer gets reward (simpler)
  Double-sided:  Both referrer and invitee get reward (higher conversion)

REWARD OPTIONS:
  [ ] Free month / credits          — direct value
  [ ] Feature unlock                — drives engagement
  [ ] Swag / status                 — community building
  [ ] Cash / gift card              — transactional, less sticky

LOOP MATH:
  Users invited per referrer:       ___
  Invite → signup conversion:       ___%
  K-factor (invites × conversion):  ___
  If K > 1: viral growth. If K < 1: referral is a channel, not a loop.
```

### Free Tool Strategy (Engineering-as-Marketing)

Build a free tool that your ICP uses, captures leads, and demonstrates your product's value:

```
FREE TOOL EVALUATION
=====================
Tool type options:
  [ ] Calculator    (ROI calculator, cost estimator, savings analyzer)
  [ ] Generator     (Template generator, name generator, copy generator)
  [ ] Analyzer      (Site audit, code quality check, security scan)
  [ ] Tester        (Speed test, compatibility check, validation tool)
  [ ] Library       (Template library, resource hub, benchmark database)
  [ ] Interactive   (Quiz, assessment, diagnostic)

EVALUATION SCORECARD:
  ICP relevance (1-5):        ___ Does your ICP actually need this?
  SEO/shareability (1-5):     ___ Will people search for or share this?
  Product bridge (1-5):       ___ Does it naturally lead to your paid product?
  Build effort (1-5 inverse): ___ Can you build it in < 2 weeks?
  TOTAL:                      ___/20 (build if 14+)
```

### 30-Day Growth Sprint Plan

```
30-DAY GROWTH SPRINT
======================
WEEK 1: Foundation
  [ ] Define aha moment and activation metric
  [ ] Instrument activation funnel (events, drop-off tracking)
  [ ] Identify and fix #1 drop-off point in onboarding
  [ ] Set baseline metrics for all AARRR stages

WEEK 2: Activation
  [ ] Reduce time-to-value by removing 1+ steps
  [ ] Add stalled-user recovery email (trigger at [X] hours)
  [ ] Test one onboarding change (welcome flow, defaults, templates)

WEEK 3: Referral + Content
  [ ] Implement basic referral mechanism (in-product or share link)
  [ ] Publish 2 pieces of content targeting ICP search queries
  [ ] Launch one free tool if scorecard ≥ 14/20

WEEK 4: Measure + Iterate
  [ ] Review activation rate change vs baseline
  [ ] Review referral K-factor
  [ ] Identify next growth lever to focus on for month 2
  [ ] Document what worked and what didn't
```

### Output
Deliver: Growth model assessment + recommended loop type + activation framework + referral loop design + free tool evaluation (if applicable) + 30-day sprint plan.

---

## Integration Notes

- **Before building:** Run `/gtm:positioning` first — everything else flows from ICP + value prop
- **Before outreach:** Run `/gtm:positioning` → `/gtm:outreach`. ICP and triggers feed directly into messaging.
- **Before launch:** Run `/gtm:landing` to CRO-audit your page, then `/seo:page` + `/geo:score` for discoverability
- **After launch:** Run `/gtm:growth` to design loops, then `/gtm:metrics` to measure them
- **Pairs with Design Thinking:** `/dt:empathize` feeds directly into ICP definition
- **Pairs with GEO:** `/geo:score` validates your launch content is AI-search-ready
- **Pairs with SEO:** `/seo:page` audits your landing page before launch

## Principles

1. **Positioning first, features second.** If you can't explain who it's for and why, building more features won't help.
2. **Two channels, not ten.** Pre-PMF, depth beats breadth. Master two channels before adding a third.
3. **Price on value, not cost.** What you charge signals what you are. Underpricing erodes trust.
4. **Measure what matters.** One north star, 5-7 supporting metrics. Everything else is noise.
5. **Launch is day one, not the finish line.** The real work starts after you ship.
6. **Personalize or don't send.** Level 3+ personalization minimum. Everything else is spam.
7. **Loops beat campaigns.** A campaign stops working when you stop spending. A loop compounds.
8. **Activation is the #1 growth lever.** Users who don't reach the aha moment will churn regardless of acquisition volume.
