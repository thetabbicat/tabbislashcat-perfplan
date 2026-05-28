---
name: perfplan
description: Extract intent from messy tasks, compress into haiku-structured executable prompts for model handoff and prompt engineering.
---
# /perfplan — Intent Compression to Haiku Prompts

## What It Does

`/perfplan` analyzes messy, verbose, or complex input and **extracts the true intent**, then structures it into **haiku-compressed executable tasks** that can be handed directly to Claude, Opus, or any other model for execution.

Instead of: "I need to build a thing that does X but also handles Y and there's this edge case with Z..."

Output: A clean, haiku-per-task structure where every line is a complete executable instruction.

## When to Use This Skill

- **Complex projects** that need clear breakdown
- **Vague briefs** that need intent extraction
- **Task handoff** to other models
- **Prompt engineering**
- **Planning avoidance**

## How It Works

### Step 1: Intent Analysis (Silent)
Read the user's input. Extract:
- Core objective
- Constraints
- Success criteria
- Context gaps

### Step 2: Haiku Structuring
For each executable task, write ONE haiku (3 lines, prioritize clarity):
- Line 1: What (action)
- Line 2: How (method/tool)
- Line 3: Why (output/result)

### Step 3: Extract Meta
- **#Role:** Who should execute this?
- **#Context:** Who reads this?
- **#Constraint:** Limits/requirements
- **#File Format:** Output structure

### Step 4: Prompt Assembly
Combine into copy-paste-ready block with success criteria.

## Example
**Input:** "I need to build a dashboard..."
**Output:** Structured haiku prompt block

## Key Principles
1. Extract intent from noise
2. Divine the character
3. One task per haiku
4. Copy-paste ready
5. No explanations in output
6. Respect constraints

## Edge Cases
- If input is already clear: Still compress it
- If input has conflicting directives: Call it out briefly
- If input is multiple projects: Run separately

## Flow
1. User sends task
2. You analyze silently
3. Output haiku-structured prompt block
4. User can immediately use it

---

## Using This Skill
`/perfplan: [paste task here]`
