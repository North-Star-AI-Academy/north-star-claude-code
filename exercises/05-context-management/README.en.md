# Level 5: Context Management — Your context window is a budget

## Goal
Understand how the context window works, when it fills up, and how to manage it efficiently.

## Theory

Claude Code has a context window of ~200K tokens. That sounds like a lot, but it fills up fast:
- Every file Claude reads: 100-5000+ tokens
- Every tool call and result: tokens
- Your entire conversation history: tokens

**The three rules:**
1. **Start every task clean** — Begin a new session (`/clear`) for each new task
2. **Compress regularly** — Use `/compact` when you notice Claude slowing down
3. **Be specific** — "Fix the bug in `src/header.tsx` line 42" beats "there's a bug somewhere"

## Exercises

### 5.1 — Checking your context status
Look at the status bar at the bottom of your terminal. You'll see:
- How many tokens you've used
- How many are left
- The percentage used

Run a few tasks and watch how the counter goes up.

### 5.2 — Experience compact
1. Ask Claude a few questions (5-10 messages)
2. Check the token counter
3. Type `/compact`
4. Watch how the counter drops

Claude compresses the conversation down to its essence — it remembers what matters and forgets the details.

### 5.3 — Working efficiently
Compare these two approaches:

**Bad** (wastes context):
```
Read all files in the exercises folder and give me a summary of each.
```

**Good** (conserves context):
```
Read exercises/05-context-management/README.md and give me the key takeaways.
```

### 5.4 — Starting a fresh session
When you're moving on to a completely new task:
1. Type `/clear` to reset the session
2. Or close Claude Code and start fresh

This gives you a clean context window of 200K tokens.

### 5.5 — Understanding sub-agents
Claude can spawn sub-agents for parallel tasks. Each sub-agent gets its own context window:

```
Research the following simultaneously:
1. The best LinkedIn post formats for B2B
2. The best times to post on LinkedIn in Europe
3. Examples of viral LinkedIn posts in the marketing niche
```

Claude sends out three sub-agents at the same time — faster and more efficient.

## Checklist
- [ ] You understand the three rules of context management
- [ ] You've used `/compact` and seen the effect
- [ ] You know when to start a new session
- [ ] You understand how sub-agents work

## Done?
Move on to Level 6: `/start-exercise 6`
