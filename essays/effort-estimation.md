---
layout: essay
type: essay
title: "Put so much Effort and Estimation into what I have one"
# All dates must be YYYY-MM-DD format!
date: 2025-12-14
published: true
labels:
  - Software Development
  - Team-Work
  - GitHub
---

# How I Effort Estimate 

My initial effort estimates were based on a combination of task familiarity, comparison to similar past tasks, and task decomposition. For example, UI-related issues such as creating or modifying pages (e.g., Landing Page, Rating Page) were estimated by comparing them to similar front-end tasks completed earlier in the project or in previous coursework. More complex tasks such as backend integration, database architecture, or CI setup were estimated higher due to uncertainty, required research, and integration risk.

As the project progressed from M1 to M3, I began using historical data from earlier milestones as a reference. For instance, tasks in M2 involving deployment and backend connections were estimated using actual effort data from M1 mockups and UI implementation, adjusted upward to account for backend complexity and debugging overhead.

# Estimation in Advance

Yes, even though many estimates were inaccurate, estimating in advance was still beneficial for planning and prioritization. For example, in M2, tasks like “Create Database Architecture” and “Implement Playwright Availability and CI” were estimated as higher effort, which helped the team schedule them earlier and avoid leaving risky work until the end of the milestone.

In M3, estimating helped identify which tasks were likely to be polish- or verification-heavy rather than coding-heavy (e.g., QA, UI consistency, final deployment). Even when the estimates were off, having a forecast helped manage expectations and distribute workload more evenly across the team.

# Tracking Effort 

Tracking actual effort was very useful, especially when comparing estimated vs. actual time. It became clear that some tasks consistently took longer than expected due to debugging, integration, or verification rather than raw coding. This insight influenced later estimates—for example, allocating more non-coding time to testing, QA, and deployment tasks in M3.

Actual effort tracking also helped with project decisions, such as identifying when a task was becoming too time-consuming and needed to be simplified or postponed, and recognizing which types of tasks (e.g., UI tweaks vs. backend integration) were more time-intensive than initially assumed.

# Tracking Actual Effort

Actual effort was tracked using a combination of: Manual time tracking (noting start and stop times when working on tasks), GitHub Project board updates, where coding and non-coding effort were logged per issue, and IDE-based activity awareness, ensuring only active coding time was counted.

Coding effort included writing, debugging, refactoring, and integrating code, while non-coding effort included planning, research, documentation, testing, and coordination. I believe the tracking was reasonably accurate, though some undercounting may have occurred during short context switches or informal discussions. Overall, the data reflects realistic effort distribution.

# Reflection 

Next time, I would: Track effort in smaller increments to reduce estimation error, separate large tasks into smaller issues to improve estimation accuracy, begin tracking non-coding effort more rigorously earlier in the project, use historical data sooner instead of relying mainly on intuition in early milestones, and these changes would likely improve both estimate quality and project predictability.

# AI Use 

Throughout the project, I used GitHub Copilot (GPT-4 model) as an AI-assisted development tool for code completion, boilerplate generation, and debugging support. Copilot was especially helpful for repetitive or well-structured tasks such as form validation logic, CRUD-style database queries, and basic API route scaffolding.

## Representative Prompts

**Prompt 1 – Prisma Schema**

// Create a Prisma schema for a Tool model with name, description,
// category, averageRating, and relationship to Review model

Prompt 2 – API Route

// POST endpoint to receive rating data and store in database using Prisma

Prompt 3 – Form Validation

// Validate email format and password length requirements in Next.js form

These prompts were typically embedded as inline comments or partial code contexts to guide Copilot’s suggestions rather than issued as standalone natural-language queries.
