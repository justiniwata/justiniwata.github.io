---
layout: essay
type: essay
title: "Final Project Idea: RateMyTool(s)"
date: 2025-11-04
labels:
  - Software Engineering
  - Nextjs
---

# Final Project Idea: RateMyTool(s)

## Overview

### The Problem
UH Manoa students are constantly searching for effective online learning resources to supplement their coursework—from video tutorials and practice platforms to AI tools and study aids. However, there is no centralized, student-driven platform where they can discover which tools actually work.

### The Solution
*RateMyTool(s)* is a community-driven review platform specifically for UH Manoa students to rate and review online learning resources, AI tools, and educational platforms. Similar to RateMyProfessor but for digital learning tools, students can search for resources by course code (e.g., **ICS 314**), category (e.g., *coding practice*, *math tutoring*, *AI assistants*), or tool name (e.g., **Khan Academy**, **ChatGPT**, **Codecademy**). Each tool profile displays aggregate ratings, detailed student reviews, and filters for specific UH Manoa courses where the tool proved helpful. Students can upvote helpful reviews, save favorite tools to their personal dashboard, and receive personalized recommendations based on their major and courses.

## Proposers
- Joseph Creollo  
- Henry Korver  
- Justin Iwata  
- Kade Komeya

## Mockup Page Ideas
- **Landing Page:** Overview of the platform's purpose, featured tools, recently reviewed resources, and trending tools among UH Manoa students. Quick search bar prominently displayed.  
- **Tool Directory / Browse Page:** Searchable and filterable catalog organized by categories (AI Tools, Video Platforms, Practice Sites, Study Aids) and UH Manoa departments/course prefixes.  
- **Individual Tool Profile Page:**  
  - Overall rating (5-star system)  
  - Student reviews with course tags  
  - Related/similar tools  
  - External link to the actual tool  
- **Add Review Page:** Form for rating a tool across multiple dimensions, tagging UH courses, writing feedback, and specifying major/year.  
- **Course-Specific Landing Pages:** Dynamic pages (e.g., `/course/ICS314`) showing highly-rated tools reviewed for that course.  
- **Admin Dashboard:** Moderation tools for flagged reviews and tool submissions.  
- **Log-In Page:** Account creation and sign-in.

## Use Case Ideas
- **New Student Discovery:** Sarah (MATH 241) finds Khan Academy and Professor Leonard's channel top-rated for calculus topics.  
- **AI Tool Comparison:** Kevin compares ChatGPT Plus vs Claude Pro for ICS homework using student reviews tagged by course.  
- **Contributing Back:** Maria tags coding practice platforms with ICS 111 and explains suitability for beginners vs interview prep.  
- **Major-Specific Recommendations:** James (Biology) sees trending tools among Biology students for BIOL 171 and CHEM 161.  
- **Course Preparation:** Alex previews tools recommended for React/Next.js before registering for ICS 314.  
- **Upvoting & Saving:** Students upvote helpful reviews and bookmark tools for later.

## Beyond the Basics — Advanced Features
- Chatbot integration to summarize site results.  
- Curated tool collections (e.g., "Best Free AI Tools for ICS Majors").  
- Side-by-side comparison tool.  
- Mobile-responsive design using Bootstrap 5.  
- User profile/dashboard showing reviews, saved tools, recommendations, and contribution stats.

## Special Sauce
- Personalized dashboard tracking reviews, saved tools, courses, and major.  
- Course-tag system to build rich metadata.  
- Reputation system based on helpful votes to aid moderation.  
- Dynamic recommendations based on user behavior.

## Learning Outcomes
This project demonstrates:
- Next.js & React proficiency (components, review forms, filters, dashboards).  
- Bootstrap 5 responsive UI.  
- GitHub collaboration and issue tracking.  
- Database integration for users, tools, reviews, ratings, and tags.  
- RESTful API routes for CRUD operations.  
- ESLint/TypeScript standards for code quality.  
- Community-focused design for UH Manoa.

## Technical Challenges
- Search and filter across multiple dimensions.  
- AI-assisted content moderation.  
- Recommendation algorithm design.  
- Intuitive UX for discovery and reviewing.  
- Duplicate prevention and database scale.

## Conclusion
This idea satisfies the project criteria: uses Next.js/React/Bootstrap/GitHub, provides personalized dashboards and recommendations, and targets the UH Manoa community for discovering effective learning resources.
