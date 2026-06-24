# The Content Engine Setup Guide

**How 9 Claude Skills run a full content system, solo.**

Built by Rananjay (@rananjayraj), The AI Driven Marketer.

---

## What this is

This is the actual system behind the post you commented on. No team, 12 hours a week, 9 Claude Skills doing the mechanical work while I keep the parts that are mine: strategy, personal stories, final edits, replying to people.

This guide walks through the loop, the 9 skills, and what each one is for. The weekly checklist (separate file) is the thing you'll actually use once this is running.

A quick note before you start: a few steps in the loop below are workflow steps, not skill installs. I've marked those clearly so you're not hunting for a skill file that doesn't exist.

---

## The loop: Plan → Create → Ship & Learn

The whole system runs in three phases, repeating every week.

**Plan** (Monday morning): figure out what to make and why.
**Create** (Monday afternoon): turn the plan into finished drafts.
**Ship & Learn** (Tuesday through Sunday): publish, reply, measure, and feed results back into next week's plan.

Here's each phase, step by step.

---

## Phase 1: Plan

### Step 1 - Content Calendar
**Skill:** `personal-content-calendar-planner`
Generates a strategic content calendar based on your content history, engagement patterns, and creator benchmarks. I check the week's planned topics and adjust for anything timely happening that week.

### Step 2 - Research & Gather
**Skill:** `competitive-ads-extractor`
Pulls and analyzes competitor ads from ad libraries (Facebook, LinkedIn, etc.) so you can see what messaging and creative angles are actually working in your space right now. I use this alongside a general scan of trending posts in my niche.

### Step 3 - Batch Ideation
**Not a separate skill.** This is Claude itself, working from what Steps 1 and 2 surfaced. I ask it to generate 10 content angles based on the calendar and research, then I pick the 4 I'll write that week. No install needed here, just a good prompt and the context from the first two steps.

---

## Phase 2: Create

### Step 4 - Draft Creation
**Skill:** `linkedin-automation-posts`
Generates LinkedIn posts using a 10-step structure (hook, pain/empathy, feature-benefit pairs, CTA, hashtags) built for automation and AI workflow content. I run this for each of the 4 picked angles, with hook variations for each.

### Step 5 - Refinement
**Skill:** `linkedin-post-reviewer`
Runs a full review pass: fact-check, rating, full rewrite, and cover image direction, all in one pass. I read the critique, make the final edits myself, and that's the post that ships.

**Running quietly underneath both Step 4 and Step 5:** `brand-voice-guidelines`. This isn't a step you run on its own, it's the consistency layer that keeps tone and terminology aligned across every draft and every rewrite. If your voice keeps drifting between posts, this is the skill to add here.

### Step 6 - Repurposing
**Skill:** `content-repurposing-engine`
Takes one finished piece of long-form content and converts it into a full distribution stack: Twitter/X threads, YouTube descriptions, newsletter sections, and more, all from the same source piece.

---

## Phase 3: Ship & Learn

### Step 7 - Daily Posting
**Not a separate skill.** This is the manual part: scheduling through Buffer (or LinkedIn's native scheduler), posting consistently at the same time, and spending the first 30 minutes after each post replying to comments. No skill replaces this step, it's where the actual relationship-building happens.

### Step 8 - Performance Analysis
**Skills:** `content-engagement-analyzer` + `data-anomaly-detective`
Two skills working together here. `content-engagement-analyzer` looks at what drove engagement across your posts (length, format, topic, timing). `data-anomaly-detective` flags anything unusual in your broader metrics (traffic, conversions, GA4 data) so you catch problems or unexpected wins early. Together they tell you what worked and what to adjust in next week's calendar.

### Step 9 - Newsletter Deep-Dive
**Skill:** `weekly-newsletter-generator`
Combines the week's best content into a recurring newsletter edition: researches supporting context, curates resources, writes a bonus actionable section, and saves a publication-ready draft. I send this to my subscriber list every week.

---

## The 9 skills at a glance

| # | Skill | Phase | What it does |
|---|---|---|---|
| 1 | `personal-content-calendar-planner` | Plan | Builds the weekly content calendar |
| 2 | `competitive-ads-extractor` | Plan | Pulls competitor ad messaging and creative patterns |
| 3 | `linkedin-automation-posts` | Create | Drafts posts using a proven 10-step structure |
| 4 | `linkedin-post-reviewer` | Create | Fact-checks, rates, and rewrites drafts |
| 5 | `brand-voice-guidelines` | Create (cross-cutting) | Keeps tone and terminology consistent across drafts |
| 6 | `content-repurposing-engine` | Create | Converts one piece into a full distribution stack |
| 7 | `content-engagement-analyzer` | Ship & Learn | Finds what drove engagement |
| 8 | `data-anomaly-detective` | Ship & Learn | Flags unusual patterns in broader metrics |
| 9 | `weekly-newsletter-generator` | Ship & Learn | Builds the weekly newsletter edition |

---

## Tools you'll still need outside Claude

These skills don't replace your stack, they run inside it. You'll still need:
- A place to hold the calendar (Notion, a spreadsheet, or similar)
- A scheduler for posting (Buffer, or your platform's native scheduler)
- A newsletter platform (Beehiiv, or your provider of choice)
- Analytics access (LinkedIn analytics export, GA4, or similar)
- Access to whichever ad libraries you want to research (Facebook Ad Library, LinkedIn Ad Library)

## Installing the skills

Each `.skill` file installs the same way any Claude skill does in your account. Where exactly that setting lives depends on whether you're in Claude.ai or Cowork, and that path has changed before as Anthropic updates the product, so check your current Settings or Capabilities menu for the add-a-skill option rather than relying on a specific click path here.

## What this guide does not include

There's no Notion template in this package yet. I'm still figuring out what's worth templating versus what just needs to live in your own calendar tool, so for now this guide and the weekly checklist are what you're getting. If a template comes together later, I'll follow up.

---

Questions on any step? Reply here or send a DM. Curious to hear how this runs for you once you've got it set up.
