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

## Integration Notes

- **Before building:** Run `/gtm:positioning` first — everything else flows from ICP + value prop
- **Pairs with Design Thinking:** `/dt:empathize` feeds directly into ICP definition
- **Pairs with GEO:** `/geo:score` validates your launch content is AI-search-ready
- **Pairs with SEO:** `/seo:page` audits your landing page before launch
- **Post-launch:** Use `/gtm:metrics` to set up your measurement framework, then track weekly

## Principles

1. **Positioning first, features second.** If you can't explain who it's for and why, building more features won't help.
2. **Two channels, not ten.** Pre-PMF, depth beats breadth. Master two channels before adding a third.
3. **Price on value, not cost.** What you charge signals what you are. Underpricing erodes trust.
4. **Measure what matters.** One north star, 5-7 supporting metrics. Everything else is noise.
5. **Launch is day one, not the finish line.** The real work starts after you ship.
