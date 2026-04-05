---
applyTo: "**/*.branch.md, **/branches/**, **/choices/**"
---

# 🌿 Branching & Choice System Instructions

Design and document meaningful player choices with real consequences.

---

## 🧭 Philosophy of Choice

> A choice that doesn't cost anything doesn't **mean** anything.
> A choice with no wrong answer isn't really a choice.

The goal is never to punish the player — it's to make them **feel the weight** of their decisions and **care about outcomes**.

---

## 📊 Choice Architecture

### The Four Types of Choices

#### 1. Value Choices (Best)
> Force the player to reveal their character's moral priorities.

```
Do you save the child or the healer who could save hundreds?
Do you tell the truth and destroy someone's hope, or lie to protect them?
Do you sacrifice your goal for a stranger's life?
```
These have no right answer. The player defines who their character IS.

#### 2. Strategic Choices (Strong)
> Different approaches with different trade-offs.

```
Sneak through and arrive fresh but uninformed.
Fight through and arrive exhausted but knowing the enemy.
Negotiate and arrive allied but indebted.
```

#### 3. Relationship Choices (Strong)
> How you treat characters shapes who stands with you.

```
Do you push Kira for information she's hiding, risking her trust?
Or do you wait, maintaining the alliance but staying blind?
```

#### 4. Information Choices (Support)
> Not all choices are moral. Some reveal story options.

```
Ask about the history (exposition + character moment)
Ask about the danger (practical info + tension)
Stay silent (character reveal + NPC reaction)
```

---

## 🌳 Branch Documentation Format

### Standard Branch Block
```markdown
## CHOICE NODE: [Unique ID]

**Scene:** [Scene name where this occurs]
**Stakes:** [What is at risk?]
**Character Position:** [Where is protagonist emotionally/physically?]

---

### Option A: [Label]
**Player says/does:** "[Text or action]"
**Immediate outcome:**
**Long-term consequence:**
**Flags set:** [Variable names to track]
**Opens path:** [What becomes available]
**Closes path:** [What becomes unavailable]

---

### Option B: [Label]
**Player says/does:** "[Text or action]"
**Immediate outcome:**
**Long-term consequence:**
**Flags set:**
**Opens path:**
**Closes path:**

---

### Option C: [Label — optional]
[Same format]

---

### Convergence Point
**Where paths rejoin:** [Scene/beat name]
**What changes between paths:** [How the world is different]
**What stays the same:** [Narrative spine maintained]
```

---

## 🔗 Consequence Tracking System

### Flag Types
```yaml
# Relationship flags
rel_kira: 0..100          # Trust level with character Kira
rel_faction_accord: -5..5  # Standing with The Accord faction

# Story state flags  
saw_massacre: true/false
knows_traitor_identity: true/false
saved_village: true/false

# Character alignment flags (avoid good/evil — use values)
values_survival_over_truth: 0..10
values_loyalty_over_justice: 0..10
uses_violence_when_convenient: 0..10
```

### Echo Moments
> Past choices must **resonate forward**. Players need to feel their decisions mattered.

Every major choice should have at least ONE echo:
- A character **references** what you did
- A **door that's open or closed** based on past choice
- An **NPC attitude shift** that's clearly tied to earlier action
- A **world state difference** the player can observe

---

## ⚖️ Choice Design Checklist

### For Every Major Choice Node:

**Before Writing:**
- [ ] What **value conflict** is at the core of this choice?
- [ ] Are all options **genuine** (none obviously correct)?
- [ ] Does each option have a **real cost**?
- [ ] What does each choice say about the **player's character**?

**While Writing:**
- [ ] Options are **concrete** (not vague)
- [ ] Consequences are **visible and felt** (not just logged)
- [ ] No option is framed as obviously good or evil
- [ ] Player agency feels **real** (not railroaded to same outcome)

**After Writing:**
- [ ] Flag variables documented in `progress.instructions.md`
- [ ] Echo moment planned for at least 1 future scene
- [ ] Convergence point identified (story continues cohesively)

---

## 🎯 Endings Architecture

### Multiple Endings Framework

Good endings aren't random — they're **earned** by accumulated choices.

```markdown
## ENDING: [Name]

**Conditions:** [Combination of flags that lead here]
**Thematic Statement:** [What this ending says about the story's theme]
**Emotional Tone:** [Bittersweet / Triumphant / Tragic / Ambiguous]

**What the Player Won:**
**What the Player Lost:**
**Final Image:** [The lasting visual/moment — what player carries out]
**Post-Credits (optional):** [Hint at what happens next in world]
```

### Ending Design Rules
- All endings should feel **earned**, not arbitrary
- No ending should be "objectively best" — each should resonate differently
- The **darkest** ending must still have dignity, not punishment
- The **best** ending must still have loss, not wish fulfillment
- Each ending reflects **who the player chose to be**, not just what they did

---

## 🚫 Branching Anti-Patterns

| Anti-Pattern | Problem | Fix |
|---|---|---|
| **Illusion of Choice** | All paths lead to identical scene | Make at least 1 meaningful difference per path |
| **Obviously Evil Option** | "Kill everyone" as a choice | Reframe as a value, not an action |
| **Consequence-free Choices** | Player ignores past choices | Add echo moments |
| **Binary Morality** | Good vs. Evil meter | Use specific value tracking instead |
| **Sudden Convergence** | Paths reunite with no acknowledgement | NPC or environment must acknowledge what happened |
