---
title: Fitness Chatbot Brief
created_date: 2026-02-13
owner: debdeepbasu
---

# Fitness chatbot (web + LLM) — brief

## Goal
Build a web-based fitness chatbot that answers common fitness questions clearly and safely, using a curated FAQ for grounding, and supporting **light personalization** (simple, safe adjustments based on basic user inputs).

This is intended as a small end-to-end agent prototype to build practical fluency in agents/tooling and document learnings (aligned to `GOALS.md`).

## Target user
- Adults who want trustworthy, practical fitness guidance without having to browse multiple sources.
- Beginners who need simple routines, basic nutrition guidance, and help getting started.
- Intermediate lifters who want reminders of best practices (progression, recovery, programming basics).

## Primary jobs-to-be-done
- Get a beginner-friendly workout plan template and understand how to progress.
- Understand fat loss vs muscle gain basics (calories, protein, training, recovery).
- Troubleshoot common situations (plateaus, soreness, missed workouts, time constraints).
- Get general form cues (non-medical, non-diagnostic) and alternatives to exercises.
- Understand recovery basics (sleep, stress, deloads) and training frequency/volume.

## Supported topics (MVP)
- **Strength training**: beginner routines, full-body vs split, progressive overload, sets/reps, rest times.
- **Nutrition basics**: calories, protein, macros basics, fiber, hydration, meal timing (general).
- **Fat loss**: sustainable deficit guidance, adherence, hunger management, steps/cardio basics.
- **Muscle gain**: surplus basics, protein targets, training volume/progression, patience.
- **Recovery**: sleep, soreness (DOMS), rest days, deload concept, stress management.
- **Habit/consistency**: building routines, motivation vs systems, tracking basics.
- **Supplements**: high-level evidence overview (e.g., protein powder, creatine, caffeine) without dosing.

## Light personalization (allowed)
The bot may ask for and use these inputs to tailor *ranges* and *options* (not prescriptions):
- Age (18+ only), sex (optional), height, weight
- Activity level (e.g., sedentary → very active)
- Training experience (beginner/intermediate)
- Goal (fat loss, muscle gain, maintenance, general fitness)
- Dietary preferences/restrictions (e.g., vegetarian) — optional
- Schedule constraints (days/week, time per session, equipment)

Outputs must be framed as:
- Ranges/starting points, with guidance to adjust based on results and well-being
- Simple templates (e.g., 3-day full body) rather than complex periodized plans
- Clear “check with a professional” guidance when appropriate

## Non-goals (explicit exclusions)
- **Medical advice**: injury diagnosis, treatment plans, medication interactions, disease-related guidance.
- **Eating disorder content**: requests that indicate disordered eating, extreme restriction, self-harm.
- **Under-18 coaching**: personalized training/nutrition for minors.
- **PED guidance**: steroid cycles, dosing, sourcing; no facilitation.
- **Highly prescriptive plans**: detailed meal plans or extreme protocols.

## Safety and refusals (high-level)
- If a user asks for injury diagnosis/medical advice: refuse and recommend a clinician/physio.
- If ED-related: refuse and offer crisis/support resources (region-appropriate if known).
- If under-18: refuse personalized coaching; provide general healthy activity guidance only.
- Supplements: allow general info; avoid dosing and contraindication claims; refuse PED guidance.

## Product principles
- **Grounded**: Prefer answering from the curated FAQ knowledge base; avoid “confident guessing.”
- **Clarify first**: Ask 1–3 targeted questions when needed (goal, experience, equipment, time).
- **Practical**: Give actionable next steps and simple templates.
- **Respectful and non-judgmental**: Avoid shame; emphasize sustainable habits.
- **Transparent**: State uncertainty and suggest credible next steps when outside scope.

## Success criteria (prototype-level)
- Users report answers are clear, actionable, and “feel safe.”
- The bot reliably refuses disallowed topics with consistent templates.
- The bot uses the FAQ as the primary source for common questions (grounding).
- A small evaluation set (test questions) passes a checklist at an acceptable rate.
