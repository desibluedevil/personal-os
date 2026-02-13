---
title: Deploy fitness chatbot prototype
category: technical
priority: P2
status: n
created_date: 2026-02-13
estimated_time: 120
resource_refs:
 - Knowledge/fitness-chatbot/prompt-policy.md
 - Knowledge/fitness-chatbot/test-questions.md
---

# Deploy fitness chatbot prototype

## Context
Deploying forces good operational habits: secrets management, logging, and a real user loop.

## Next Actions
- [ ] Choose hosting (default suggestion: Vercel for Next.js).
- [ ] Set up environment secrets for LLM API key (never commit secrets).
- [ ] Add a basic “Safety & limitations” note in the UI:
  - Not medical advice; no injury diagnosis
  - Refusal topics
- [ ] Add rate limiting and basic abuse protection.
- [ ] Validate refusal behavior on the deployed version using `test-questions.md`.
- [ ] Share the URL with 2–3 friendly testers for quick feedback.

## Progress Log
- 2026-02-13: Task created from spec plan.
