---
name: viral-product-reviewer
description: Audit a landing page, website, or codebase against Marc Lou's "32 Principles of a Viral Product". Use when the user wants to review, score, or improve a product's virality, marketing copy, pricing, or landing page design based on these 32 principles.
---

# Viral Product Reviewer

This skill audits a product (via URL, screenshots, or codebase) against Marc Lou's 32 Principles of a Viral Product, generating a comprehensive Markdown report with actionable improvements for indie hackers and builders.

## Workflow

When triggered to review a product, follow these steps:

### 1. Gather Information
- **If given a URL**: Use browser tools or `webpage_extract` to read the landing page copy, pricing, hero section, and OG images.
- **If given a codebase**: Use `match` and `file` tools to find and read marketing-facing pages (e.g., `index.html`, `page.tsx`, `pricing.tsx`), layout files (for headers/footers), and metadata configurations (for OG images and title tags).
- **If given screenshots**: Use `file` with the `view` action to visually analyze the design, colors, hero section, and layout.

### 2. Load the 32 Principles
Read the full list of principles to ensure accurate scoring:
```bash
# Read the reference file
/home/ubuntu/skills/viral-product-reviewer/references/32_principles.md
```

### 3. Conduct the Audit
Evaluate the gathered information against all 32 principles.
- For each principle, determine if the product passes (✅), fails (❌), or if there isn't enough information to judge (⚠️).
- Formulate specific, actionable feedback for any failed principles.
- Identify the top 3-5 priority improvements that will move the needle the most.

### 4. Generate the Report
Create a Markdown report using the provided template:
```bash
# Read the template file
/home/ubuntu/skills/viral-product-reviewer/templates/report_template.md
```
- Fill out the template completely.
- Save the final report as a `.md` file in the working directory (e.g., `viral_product_review.md`).

### 5. Deliver the Results
Use the `message` tool with `type: result` to deliver the final Markdown report file to the user as an attachment.
