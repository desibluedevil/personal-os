---
title: Fitness Chatbot FAQ (Grounding Knowledge Base)
created_date: 2026-02-13
owner: debdeepbasu
---

# Fitness chatbot — FAQ knowledge base

Use this as the primary grounding source for common questions. Each entry includes:
- **Tags** for retrieval
- **When_to_clarify**: follow-up questions to ask before giving advice
- **Answer**: a safe, practical response template

## How to use this FAQ (for the assistant)
- Prefer **FAQ answers** over general web knowledge.
- If the question is missing key context, ask the minimum number of clarifying questions (1–3).
- If the question falls under safety exclusions (injury diagnosis, ED content, under-18 coaching, PEDs), follow `prompt-policy.md`.

---

## Training basics

### Q: What’s the best workout routine for a beginner?
**Tags**: `training`, `beginner`, `routine`, `full_body`
**When_to_clarify**:
- How many days/week can you train?
- Do you have equipment (gym / dumbbells / bodyweight)?
- Any movement limitations or medical constraints? (If yes: safety handoff)
**Answer**:
- A great default is **3 days/week full-body** focusing on squat/hinge/push/pull/carry patterns.
- Keep it simple: 5–7 exercises/session, 2–3 sets each, 6–12 reps, leaving **1–3 reps in reserve**.
- Progress by adding **a little weight or reps** each week when you hit the top of the rep range with good form.
- Example template (gym):
  - Squat or leg press
  - Romanian deadlift or hip hinge
  - Bench press or push-up
  - Row or lat pulldown
  - Overhead press (optional)
  - Plank or dead bug
  - Optional: curls/triceps 1–2 sets

### Q: Full-body vs split—what should I do?
**Tags**: `training`, `programming`, `beginner`, `frequency`
**When_to_clarify**:
- Days/week available?
- Primary goal (strength, muscle, fat loss, general fitness)?
**Answer**:
- **Full-body** is usually best for beginners or 2–3 days/week: frequent practice, simple progression.
- **Upper/lower** or **push/pull/legs** can work well if you can train 4–6 days/week.
- The “best” split is the one you can do consistently while hitting each muscle group **~2x/week** (often) with manageable fatigue.

### Q: How many sets and reps should I do?
**Tags**: `training`, `hypertrophy`, `strength`, `sets_reps`
**When_to_clarify**:
- Beginner vs intermediate?
- Goal: strength vs muscle vs mixed?
**Answer**:
- For general fitness and muscle: **6–12 reps** for most lifts, **2–4 sets**.
- For strength: include some heavier work like **3–6 reps** on key lifts, plus back-off sets.
- A simple weekly target for growth is roughly **8–15 hard sets per muscle group per week**, adjusted to recovery.
- Most sets should end with **1–3 reps in reserve**; go to failure sparingly.

### Q: What is progressive overload?
**Tags**: `training`, `progression`, `beginner`
**When_to_clarify**: none
**Answer**:
- Progressive overload means gradually increasing training demand over time.
- Practical ways:
  - Add **reps** (e.g., 8 → 10 → 12)
  - Add **weight** (small jumps)
  - Add **sets** (2 → 3)
  - Improve **range of motion** or **control**
- Keep form consistent; progress should be small and repeatable.

### Q: How long should I rest between sets?
**Tags**: `training`, `rest_times`, `strength`
**When_to_clarify**:
- What exercise type (heavy compound vs isolation)?
**Answer**:
- Heavy compounds (squat/bench/deadlift/rows): **2–4 minutes**.
- Isolation work (curls/lateral raises): **60–120 seconds**.
- Rest enough to keep performance and technique solid.

---

## Fat loss

### Q: How do I lose fat?
**Tags**: `fat_loss`, `nutrition`, `calories`, `beginner`
**When_to_clarify**:
- Age 18+? (if minor: refuse personalization)
- Goal timeline (gentle vs aggressive)?
- Current activity and training?
**Answer**:
- Fat loss requires a sustained **calorie deficit**.
- Best “big rocks”:
  - Protein at each meal
  - High-fiber foods (fruit/veg/whole grains/legumes)
  - Daily steps (e.g., a step goal you can maintain)
  - Strength training to maintain muscle
  - Sleep and stress management
- A sustainable starting point is aiming for **~0.25–0.75% bodyweight loss per week**; adjust based on results and energy.

### Q: Do I need to do cardio to lose weight?
**Tags**: `fat_loss`, `cardio`, `training`
**When_to_clarify**:
- What do you enjoy and can sustain?
**Answer**:
- Cardio is helpful for health and can increase calorie burn, but it’s **not required**.
- Many people do best with a combo: strength training + steps + some cardio they enjoy.
- If adding cardio increases hunger too much, adjust intensity/duration or focus on steps.

### Q: Why am I not losing weight even though I’m eating less?
**Tags**: `fat_loss`, `plateau`, `troubleshooting`
**When_to_clarify**:
- How long has the plateau been (weeks)?
- Are measurements only scale weight, or also waist/photos?
- Tracking method (weighing food vs estimates)?
**Answer**:
- Common reasons:
  - Intake is higher than estimated (liquid calories, snacks, portions)
  - Lower activity (less movement when dieting)
  - Water retention (stress, sodium, menstrual cycle, hard training)
  - Too short a timeframe (need 2–4 weeks to see trend)
- Troubleshoot:
  - Track consistently for 1–2 weeks
  - Increase steps modestly
  - Ensure protein + fiber
  - Use weekly average weight, not daily fluctuations

---

## Muscle gain

### Q: How do I build muscle?
**Tags**: `muscle_gain`, `training`, `nutrition`, `hypertrophy`
**When_to_clarify**:
- Training age and current schedule?
- Equipment access?
- Any dietary constraints?
**Answer**:
- Core requirements:
  - Progressive strength training
  - Enough protein and total calories (often slight surplus)
  - Enough sleep/recovery
- Practical guidance:
  - Train each muscle group **~2x/week**
  - Keep most sets 1–3 reps from failure
  - Prioritize consistent weekly volume you can recover from
  - Protein spread across the day (e.g., 3–4 meals with protein)

### Q: Should I bulk or cut first?
**Tags**: `muscle_gain`, `fat_loss`, `beginner`
**When_to_clarify**:
- Current body comp goals and comfort level?
- Training experience?
**Answer**:
- Beginners can often do a “recomp” phase: build strength and muscle while slowly losing fat.
- If you feel you have significant fat to lose: start with a gentle deficit and strength training.
- If you’re already lean and want size: small surplus + structured training.
- Most important is a plan you’ll stick with for **8–12 weeks** before changing.

---

## Nutrition basics

### Q: How much protein do I need?
**Tags**: `nutrition`, `protein`, `fat_loss`, `muscle_gain`
**When_to_clarify**:
- Bodyweight (optional), goal (fat loss vs muscle gain), dietary preference
**Answer**:
- A practical target for many active adults is **1.6–2.2 g/kg/day** (or roughly **0.7–1.0 g/lb/day**).
- If you’re dieting, staying toward the higher end can help preserve muscle and manage hunger.
- Spread protein over meals; choose sources you tolerate and enjoy.

### Q: Are carbs bad?
**Tags**: `nutrition`, `carbs`, `myths`
**When_to_clarify**: none
**Answer**:
- Carbs aren’t “bad.” They’re a primary fuel, especially for training.
- Quality and total intake matter: fruits, veggies, legumes, whole grains often help performance and satiety.
- Some people prefer lower-carb for appetite control; the best diet is one you can sustain while meeting protein and calorie goals.

### Q: Should I count calories?
**Tags**: `nutrition`, `calories`, `tracking`
**When_to_clarify**:
- User preference and history (avoid if disordered eating concerns)
**Answer**:
- Calorie counting is a tool, not a requirement.
- Alternatives:
  - Portion-based approach (protein + veg each meal)
  - Consistent meal patterns
  - Tracking only protein and steps
- If counting calories increases anxiety or obsessive behavior, avoid it and use simpler habits.

---

## Recovery

### Q: How much sleep do I need for fitness results?
**Tags**: `recovery`, `sleep`, `performance`
**When_to_clarify**: none
**Answer**:
- Most adults do best with **7–9 hours**.
- Sleep supports muscle recovery, appetite regulation, mood, and performance.
- If improving sleep is hard, start with: consistent wake time, morning light, reduced late caffeine, and a short wind-down routine.

### Q: Is soreness a good sign?
**Tags**: `recovery`, `doms`, `training`
**When_to_clarify**:
- New program? Very sore limiting movement?
**Answer**:
- Mild soreness can be normal (especially with new exercises), but it’s **not required** for progress.
- Extreme soreness that disrupts daily movement suggests too much volume/intensity too soon.
- Progress by gradually increasing workload; prioritize good technique and recovery.

---

## Supplements (high-level, no dosing)

### Q: Do I need supplements?
**Tags**: `supplements`, `nutrition`, `beginner`
**When_to_clarify**:
- Dietary preference and constraints?
**Answer**:
- Supplements are optional. Focus first on training consistency, protein, calories, sleep.
- Common, generally well-supported options (high-level):
  - Protein powder (convenience)
  - Creatine (performance support)
  - Caffeine (performance, if tolerated)
- If you have medical conditions, are pregnant, or take medications, talk to a clinician before adding supplements.

---

## Equipment and constraints

### Q: I only have 20 minutes—what should I do?
**Tags**: `training`, `time_constraint`, `beginner`
**When_to_clarify**:
- Home vs gym?
- 2–4 days/week?
**Answer**:
- Use short full-body sessions:
  - 2–3 compound movements + 1 core/carry
  - Superset push/pull to save time (if safe)
  - Keep 1–2 warm-up sets then 2 hard sets
- Consistency beats perfect programming; a simple plan done weekly will outperform sporadic longer workouts.

### Q: Home workout with dumbbells only?
**Tags**: `training`, `home`, `dumbbells`
**When_to_clarify**:
- Dumbbell weights available?
**Answer**:
- Build around patterns:
  - Squat: goblet squat / split squat
  - Hinge: RDL
  - Push: floor press / push-ups
  - Pull: one-arm row
  - Core: plank variations
- Progress with reps, slower tempo, more sets, or unilateral variations if weights are limited.
