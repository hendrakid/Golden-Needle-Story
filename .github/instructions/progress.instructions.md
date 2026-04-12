---
applyTo: "**/*.story.md, **/story/**, **/narrative/**, **/scenes/**"
---

# 📈 Story Progress Instructions

Track and maintain the overall narrative arc, act structure, and story momentum.

---

## 🗺️ Story Arc Structure

This project follows a **modified Hero's Journey** with player agency at each threshold:

```
ACT 1 — THE ORDINARY WORLD
  ├── Hook Scene (0–5 min)
  ├── World Introduction
  ├── Inciting Incident
  └── Call to Adventure / First Choice ← MAJOR BRANCH POINT

ACT 2A — DESCENT
  ├── New World Rules Established
  ├── First Allies & Enemies
  ├── Midpoint Revelation (changes everything)
  └── Dark Night of the Soul ← MAJOR BRANCH POINT

ACT 2B — ORDEAL
  ├── Consequence of Midpoint
  ├── Allies Tested
  ├── Point of No Return
  └── Black Moment (lowest point) ← MAJOR BRANCH POINT

ACT 3 — RETURN
  ├── Climax Setup
  ├── Final Confrontation
  ├── Resolution (multiple endings)
  └── Epilogue / Denouement
```

---

## 📊 Current Progress Tracker

> **Update this section as the story develops.**

```yaml
current_act: "ACT 1"
current_scene: "Hook Scene"
scenes_completed: []
major_choices_made: []
active_threads:
  - name: "Main Quest"
    status: "active"
    last_beat: ""
  - name: "Character Arc - Protagonist"
    status: "active"
    last_beat: ""
pending_payoffs: []
foreshadowing_planted: []
```

---

## 📌 Scene Completion Checklist

Before marking a scene complete, verify:

- [ ] Scene serves a clear **narrative purpose**
- [ ] **Emotional beat** is landed (joy, dread, hope, grief, etc.)
- [ ] At least one piece of **character development** occurred
- [ ] **World** feels more alive than before this scene
- [ ] Any **promises made** to the player (tension, mystery) are tracked
- [ ] **Continuity** with previous scenes confirmed
- [ ] Branch consequences are logged (if applicable)

---

## 🔮 Foreshadowing Log

Track planted seeds to ensure payoff:

| Scene Planted | Element | Intended Payoff Scene | Status |
|---------------|---------|----------------------|--------|
| - | - | - | Pending |

---

## ⚡ Story Momentum Rules

### Momentum Killers (Avoid)
- Two low-tension scenes back-to-back
- Characters discussing past events without present stakes
- Explanations that stop all story movement
- Backtracking without character purpose

### Momentum Builders (Prefer)
- End every scene with an **unresolved question**
- Introduce complications **before** resolving existing ones
- Let characters make decisions **under pressure**
- Reveal character through **action**, not backstory monologue

---

## 🔗 Thread Management

### Active Threads
Track every open story thread. Nothing should be left dangling:

```
Thread: [Name]
Status: Active / Dormant / Resolved
Introduced: [Scene name]
Expected Resolution: [Act/Scene]
Current State: [Brief description]
```

### Resolution Deadlines
- Act 1 threads → Must resolve or escalate by Act 2B
- Act 2 threads → Must resolve by Act 3 climax
- Side threads → Can resolve in epilogue, but must acknowledge

---

## 🎭 Emotional Beat Tracker

Ensure variety in emotional beats across the story:

| Beat Type | Last Used | Frequency Target |
|-----------|-----------|-----------------|
| Wonder/Discovery | - | Every 3-4 scenes |
| Dread/Tension | - | Every 2-3 scenes |
| Hope/Relief | - | Every 4-5 scenes |
| Grief/Loss | - | Once per act |
| Joy/Triumph | - | Once per act |
| Betrayal/Shock | - | Once per major act |

---

## 🚀 Pacing Directives for Copilot

When asked to write a new scene:
1. Check `current_act` and `current_scene` above
2. Identify the **dominant emotion** this scene should evoke
3. Ensure there's an **open hook** at the scene's end
4. Update `scenes_completed` after writing
5. Log any new `foreshadowing_planted`

---

## ✅ Quest Acceptance Marker

When a scene includes the protagonist Sulung receiving or accepting a quest, the scene text must include a visible, machine-friendly marker using the exact format below:

- - QUEST [ID-Title] ACCEPTED -

Examples:
- - QUEST Q002-Selamatkan-Bungsu ACCEPTED -
- - QUEST SQ002-Kalahkan-Slime ACCEPTED -

Guidelines:
- Place the marker immediately after the acceptance beat as a standalone line so tools and reviewers can detect it reliably.
- Use the quest's ID followed by a hyphen and a short title (replace spaces with hyphens). Prefer the same kebab-title used in the quest filename when possible.
- Keep the whole marker on one line and use uppercase `QUEST` and `ACCEPTED` exactly as shown.
- Update `active_threads` with the quest name/status and add any relevant flags to `major_choices_made`.
- When applicable, create or update the corresponding quest file in `story/quests/` (follow existing naming conventions) and reference the quest ID and title used in the marker.

This marker is required for all scenes where Sulung explicitly accepts a quest.
