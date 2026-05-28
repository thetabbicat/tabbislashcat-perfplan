# /perfplan

> intent extraction — /perfplan mode. spun from /infant by UaZit/@tabbislashcat. turns messy tasks into haiku-structured prompts. a seed knows its dirt. perfplan finds the seed, shapes the dirt, hands you the map. no wasted token. no wasted step.

**perfplan** is a skill that extracts core intent from messy or verbose task descriptions and compresses them into **haiku-structured executable prompts** — perfect for model handoff, prompt engineering, and multi-step agentic flow.

## what it does

no noise. no fluff. signal shaped for action. copy. paste. done.

- extracts true intent from complex, vague, or rambling input
- structures tasks into haiku-compressed executable blocks (3 lines each)
- adds meta context: #Role, #Context, #Constraint, #File Format
- outputs copy-paste-ready prompts for any model (claude, opus, mistral, etc.)

## when to use

- complex projects needing clear breakdown
- vague briefs requiring intent extraction
- task handoff to other models
- prompt engineering for external LLM calls
- compressing big ideas into small, clear steps

## trigger

`/perfplan: [your task here]`

or simply mention "haiku this", "compress my task", or "intent extraction".

## example

**input:**
```
"I need to build a dashboard for my music streaming data. It should show plays over time, top tracks, listener growth. Make it fast though, don't overthink it. And I want it connected to my PocketBase somehow. Oh, also it needs to be pretty with my brand colors."
```

**output:**
```
#Role:
You are a product-minded full-stack developer who ships fast and values open-source elegance.

#Context:
This is for a solo creator building a music analytics tool. They're connected to PocketBase and their own thaypley brand.

#Constraint:
Keep under 400 tokens. Use only React + Recharts + PocketBase (no paid services).

#File Format:
Markdown haiku stack. Copy-paste ready.

=== DASHBOARD BUILD PLAN ===

TASKS:
1. Schema the data
   Extract plays timeline
   Count tracks & listeners

2. Fetch and shape it
   Query PocketBase API
   Aggregate metrics

3. Build the UI
   React + Recharts charts
   Brand color palette

4. Connect and verify
   Test data flow end-to-end
   Performance check

SUCCESS: Dashboard loads <2s, displays plays/tracks/growth, uses brand colors, syncs with PocketBase.
```

## movement modes

- **listen** — extract intent: "3 objectives found, constraints: none, proceed?"
- **carve** — haiku compression: "task 1 → task 2 → task 3"
- **frame** — meta extraction: "#Role: builder. #Context: thaypley. #Constraint: <500 tokens"
- **ship** — prompt assembly: "copy-paste ready. execute."

## philosophy

no noise. no fluff. signal shaped for action. copy. paste. done.

## installation

this is a skill for le chat (mistral ai). to use:

1. load the skill with `/perfplan` or by invoking intent compression
2. paste your messy task
3. receive haiku-structured, copy-paste-ready output
4. hand off to any model or use directly

## license

Apache 2.0 — permissive, patent grant, contributor-friendly.

Copyright (c) 2026 Stalph LLC. All rights reserved.

## family

part of the thaypley empire — a creator-owned constellation of apps, instruments, and platforms. see [thaypley(webiverse)](https://thaypley.com) for the full universe.
