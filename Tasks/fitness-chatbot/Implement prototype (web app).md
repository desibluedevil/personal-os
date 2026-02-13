---
title: Implement fitness chatbot prototype (web app)
category: technical
priority: P2
status: n
created_date: 2026-02-13
estimated_time: 360
resource_refs:
 - Knowledge/fitness-chatbot/brief.md
 - Knowledge/fitness-chatbot/faq.md
 - Knowledge/fitness-chatbot/prompt-policy.md
 - Knowledge/fitness-chatbot/test-questions.md
---

# Implement fitness chatbot prototype (web app)

## Context
Supports `GOALS.md`: ship a small agent prototype end-to-end and document learnings.

Prototype requirements:
- Web chat UI
- LLM via API
- Ground answers in `Knowledge/fitness-chatbot/faq.md`
- Enforce safety policies in `prompt-policy.md`
- Support light personalization (safe ranges, templates)

## Next Actions
- [ ] Create a new separate repo (or sibling folder) for the runnable app (keep this repo as the spec + task tracker).
- [ ] Pick stack (suggested default): Next.js + simple server route for chat.
- [ ] Implement retrieval over `faq.md` (simple chunking + vector store or keyword match for MVP).
- [ ] Implement prompt composition:
  - System: policy + tone
  - Developer: grounding rules + refusal templates
  - User: message
  - Retrieved FAQ snippets: included as context
- [ ] Add a safety gate:
  - Detect disallowed topics (medical diagnosis, ED, under-18, PEDs)
  - Route to refusal templates
- [ ] Add basic telemetry (privacy-safe): category + whether refusal triggered (no identifying data).
- [ ] Run the manual eval set in `test-questions.md` and note failures.

## Progress Log
- 2026-02-13: Task created from spec plan.
