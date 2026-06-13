# Viral Product Reviewer — Agent Skill

[![skills.sh](https://skills.sh/b/galnaaman/viral-product-reviewer)](https://skills.sh/galnaaman/viral-product-reviewer)

Audit any landing page, website, or codebase against **Marc Lou's 32 Principles of a Viral Product** and get a scored Markdown report with prioritized, actionable improvements.

Built for **indie hackers and builders** who want to ship products that actually spread.

---

## Install

```bash
npx skills add galnaaman/viral-product-reviewer
```

---

## What It Does

- Accepts a **URL**, **codebase path**, or **screenshots** as input
- Reads all marketing-facing pages: landing page copy, hero section, pricing, CTAs, OG images, footer
- Scores your product against all 32 principles: ✅ Pass / ❌ Fail / ⚠️ Unclear
- Delivers a full Markdown report with your score, top priority fixes, and per-principle feedback

---

## How to Use

Once installed, trigger it by saying things like:

- *"Review my landing page against the 32 principles"* + paste a URL
- *"Audit my codebase for virality"* + point to your project folder
- *"Score my product page"* + drop in screenshots

---

## The 32 Principles

Based on Marc Lou's article: [32 Principles of a Viral Product](https://x.com/i/web/status/2065385672991752210)

| # | Principle |
|---|-----------|
| 1 | No free plan |
| 3 | Numbers, not adjectives |
| 7 | Headline a fifth grader can understand |
| 8 | Hard paywall |
| 20 | Can be sold from the hero section alone |
| 22 | One call to action |
| 28 | CTA says what happens next |
| 29 | Launches with testimonials |
| … | All 32 principles covered |

---

## Skill Structure

```
skills/
└── viral-product-reviewer/
    ├── SKILL.md                    # Core skill instructions
    ├── references/
    │   └── 32_principles.md        # Full list of all 32 principles
    └── templates/
        └── report_template.md      # Pre-structured audit report template
```

---

## Credits

This skill is based entirely on the original article **[32 Principles of a Viral Product](https://x.com/i/web/status/2065385672991752210)** by **[Marc Lou](https://marclou.com)** ([@marclou](https://x.com/marclou)).

Marc Lou is an indie hacker who has built and shipped 35+ products in public over 5 years. His principles come from watching hundreds of launches make $0 — and a few reach millions of people. Follow his work at [marclou.com](https://marclou.com) and on [X/Twitter](https://x.com/marclou).
