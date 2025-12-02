---
layout: essay
type: essay
title: "Design Patterns: It look's Nice!!!"
# All dates must be YYYY-MM-DD format!
date: 2025-12-02
published: true
labels:
  - Software Development
  - Final Project
  - Design
  - Following Instructions
  - Working Together
---

<img width="200px" class="rounded float-start pe-4" src="../img/ratemytools_diagram.png">

## Introduction

When people imagine building a web app, they often picture typing out features one by one, like stacking blocks until a site appears. But real software—especially something meant for thousands of students—needs more than pieces placed together. It needs structure, rules, and blueprints just like a growing city. This is where design patterns come in: they are the architectural logic behind software, the reusable solutions that make a system stable even as new features, pages, or interactions pile on. I didn’t fully understand how important these patterns were until my team built our final project, RateMyTool(s), a student-driven platform for reviewing online learning tools. What looked like simple pages and forms on the surface quietly depended on deep, well-established design patterns underneath.

## The Idea of Designing Software

Design patterns are the “city planning” of code. They aren’t copy-and-paste code snippets but reusable ways to solve common problems—how to create objects, how to organize data, how to manage user flow, or how to simplify connections between components. Just like every city reuses basic designs for roads, bridges, and neighborhoods, software reuses proven solutions like Controllers, Factories, Adapters, and Observers. These patterns keep the entire system from falling apart as it grows. Without them, even a small app becomes unpredictable, with files depending on each other in messy ways. With them, code becomes modular, expandable, and understandable—not only to the person who wrote it, but to anyone who joins the project later. They are the quiet backbone that holds every modern application upright.

## Relations to Final Project

When we built RateMyTool(s), we were basically designing a small digital city for UH Manoa students—a place with profile pages, search tools, review forms, filters, and dynamic routing. And just like a city, the system needed order. For example, every time a user searched for a tool, opened a profile page, or submitted a review, the request moved through a predictable pipeline. That pipeline followed the Model–View–Controller pattern (MVC), even though we never explicitly said it. The Models (Prisma schemas) defined how data lived in the database. The Views (React pages and components) displayed what the user sees. And the Controllers (API routes) handled user actions like posting reviews or fetching tool data.

RateMyTool(s) also depended heavily on the Repository Pattern, because our Prisma client acted as a clean interface for database access. Instead of writing raw SQL everywhere, we used consistent functions like prisma.tool.findMany() or prisma.review.create(). This separation kept our logic clean and made the system easier to debug and expand.

And whenever the interface needed to respond to changing user actions—typing in search, updating filters, or loading dynamic course pages—we relied on the Observer Pattern, built naturally into React’s state system. Components “reacted” to changes in state or props, updating instantly like a system of interconnected traffic lights.

##  Design Patterns that Help our App 

Several classic design patterns appeared clearly in our final implementation:

1. Factory Pattern (Tool & Review Creation)

Whenever the system created new tools, reviews, or user entries, it used clean, encapsulated creation logic through Prisma. This mirrors the Factory Pattern: you request an object, and the system builds it correctly without exposing the construction details.

2. MVC Pattern (Global Structure of the App)

The entire site—from landing page to profile pages—follows MVC.

Models: Prisma schema + PostgreSQL database

Views: Next.js / React UI components

Controllers: API routes that connect user actions to the database

This pattern kept our roles and responsibilities clean.

3. Observer Pattern (State-Based UI Updates)

React components update automatically when state changes. This is the Observer Pattern in action: components “subscribe” to data, and when the data changes, the UI updates without us needing to manually rewrite anything.

4. Singleton Pattern (Database Connection)

Prisma uses a single shared database instance to prevent connection overload. This is a textbook use of the Singleton Pattern—ensuring only one global database connection is ever active.

5. Repository Pattern (Database Abstraction)

All interactions with PostgreSQL go through structured Prisma calls, keeping database logic separate from UI logic. This made our code more maintainable and less error-prone.

These patterns didn’t just make RateMyTool(s) work—they made it scalable, readable, and easy for the entire team to collaborate on.

## Overall Conclusion 

Looking back, design patterns weren’t just academic concepts—they were the invisible city planning that kept RateMyTool(s) from collapsing into a maze of tangled scripts and unpredictable behavior. They helped us divide work across team members, ensured our database stayed organized, and made the interface feel responsive and consistent. If I were asked in an interview what design patterns are and which ones I used, I’d say they’re reusable architectural solutions that help software grow safely—and that our project used MVC, Factory, Observer, Singleton, and Repository patterns throughout development. More importantly, I’d explain that these patterns turned a student idea into a real, functional platform. They taught me that good code isn’t just written—it’s designed.
