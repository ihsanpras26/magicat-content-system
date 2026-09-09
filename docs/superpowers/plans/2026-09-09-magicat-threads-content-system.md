# Magicat Threads Content System Implementation Plan

> **For agentic workers:** Implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build an Obsidian-compatible content and sales operating system for Magicat, including a 30-day Threads launch calendar and ready-to-edit copy.

**Architecture:** Plain Markdown files form a portable vault. Brand and product truth files are the source of truth; templates standardize production; daily content notes link back to the calendar; sales and metrics files complete the conversion and feedback loops.

**Tech Stack:** Markdown, YAML frontmatter, Obsidian core features, PowerShell verification scripts

**Spec:** `docs/superpowers/specs/2026-09-09-magicat-threads-content-system-design.md`

## Global Constraints

- Use natural Indonesian with a curious-friend voice.
- Use `aku` for experiments and `Magicat` for policies and support.
- Product price is Rp49.000.
- Never request a password, OTP, recovery code, or session cookie.
- Describe the source as an official Google x Jio program, not Magicat as an official partner.
- Coverage remedy order is restoration, replacement, then prorated refund.
- Flow-specific facts must remain explicit fill-in fields until a real asset exists.
- Use plain Markdown and Obsidian core features; do not add third-party plugins or API keys.

---

### Task 1: Vault Foundation and Brand Truth

**Files:**
- Create: `.obsidian/app.json`
- Create: `.obsidian/core-plugins.json`
- Create: `00 Dashboard/Content Dashboard.md`
- Create: `01 Brand/Positioning.md`
- Create: `01 Brand/Voice Guide.md`
- Create: `01 Brand/Product Facts.md`
- Create: `01 Brand/Claims Allowed.md`
- Create: `01 Brand/Profile Setup.md`

**Interfaces:**
- Consumes: approved design specification
- Produces: canonical positioning, voice, profile, product facts, and claim constraints

- [ ] Create the Obsidian configuration and folders.
- [ ] Write each brand source-of-truth note with links to its related notes.
- [ ] Confirm the profile copy uses `DM "GEMINI"` and does not imply official-partner status.
- [ ] Search brand notes for prohibited claims and credential requests.

### Task 2: Customer Protection and Sales Operations

**Files:**
- Create: `01 Brand/Offer and Guarantee.md`
- Create: `05 Sales/DM Scripts.md`
- Create: `05 Sales/FAQ.md`
- Create: `05 Sales/Objections.md`
- Create: `05 Sales/Safe Activation SOP.md`
- Create: `05 Sales/Order Tracker.md`
- Create: `05 Sales/Testimonials.md`

**Interfaces:**
- Consumes: `Product Facts.md`, `Claims Allowed.md`
- Produces: consistent inquiry-to-support flow and customer-facing coverage terms

- [ ] Define restoration, replacement, and prorated-refund remedies.
- [ ] Write scripts for inquiry, qualification, QRIS, activation, support, and testimonial consent.
- [ ] Write a safe activation procedure that explicitly rejects credentials and OTPs.
- [ ] Verify price, response targets, exclusions, and refund formula are consistent.

### Task 3: Content Production System

**Files:**
- Create: `02 Ideas/Content Inbox.md`
- Create: `02 Ideas/Audience Questions.md`
- Create: `02 Ideas/Hook Bank.md`
- Create: `02 Ideas/CTA Bank.md`
- Create: `02 Ideas/Reply Playbook.md`
- Create: `Templates/Content Post.md`
- Create: `Templates/Flow Experiment.md`
- Create: `Templates/Weekly Plan.md`
- Create: `Templates/Customer Insight.md`
- Create: `04 Flow Lab/Prompt Library/Flow Prompt Framework.md`
- Create: `04 Flow Lab/Prompt Products/Prompt Pack Blueprint.md`
- Create: `04 Flow Lab/Failed Results/Failure Library.md`

**Interfaces:**
- Consumes: brand truth and CTA rules
- Produces: reusable hooks, CTAs, replies, prompts, and production templates

- [ ] Write hook and CTA banks grouped by intent.
- [ ] Write reply guidance that prioritizes useful conversation over engagement bait.
- [ ] Create content and Flow templates with required factual-review fields.
- [ ] Create a productizable Flow prompt framework and failure taxonomy.

### Task 4: Thirty-Day Launch Calendar and Copy

**Files:**
- Create: `00 Dashboard/30-Day Calendar.md`
- Create: `03 Content/Ready/Day 01.md` through `Day 30.md`
- Create: `03 Content/Ready/Pinned 01 - Perkenalan.md`
- Create: `03 Content/Ready/Pinned 02 - Showcase Flow.md`
- Create: `03 Content/Ready/Pinned 03 - Gemini Offer.md`

**Interfaces:**
- Consumes: content templates, hooks, CTAs, product facts, and claims
- Produces: thirty scheduled posts and three profile pins

- [ ] Assign each day a pillar, format, goal, CTA, and readiness state.
- [ ] Write complete natural-language copy for text-led posts.
- [ ] Write fill-in drafts for media-dependent posts without inventing experiment results.
- [ ] Link every calendar row to its content note.
- [ ] Verify the mix includes eight Flow showcases and balanced sales frequency.

### Task 5: Measurement, Reader Test, and Final Audit

**Files:**
- Create: `00 Dashboard/Weekly Review.md`
- Create: `06 Metrics/Weekly Metrics.md`
- Create: `06 Metrics/Content Learnings.md`
- Create: `06 Metrics/30-Day Scorecard.md`
- Create: `README.md`

**Interfaces:**
- Consumes: all vault notes
- Produces: operating instructions, measurement loop, and verification record

- [ ] Write formulas and definitions for views, reply rate, qualified DMs, conversion, and coverage rate.
- [ ] Write a weekly decision process for continue, improve, recycle, or stop.
- [ ] Verify all expected files exist and all content notes have YAML frontmatter.
- [ ] Verify exactly thirty numbered daily notes and eight Flow showcase assignments.
- [ ] Scan for prohibited claims, accidental credential requests, unsupported testimonials, and unresolved generic placeholders.
- [ ] Run a fresh-reader review of the profile, offer, activation, coverage, and next action.
