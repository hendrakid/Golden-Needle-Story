---
applyTo: "**/*.quest.md, **/quests/**, **/missions/**, **/tasks/**"
---

# ⚔️ Quest Design Instructions

Panduan untuk merancang quest yang narratively meaningful, mechanically satisfying, dan emotionally resonant — bukan sekadar checklist objectives.

---

## 🧭 Philosophy of Quest Design

> **Quest terbaik bukan tentang apa yang harus dilakukan player.**
> Quest terbaik tentang **siapa player menjadi** setelah menyelesaikannya.

Setiap quest harus menjawab tiga pertanyaan:
1. **Mengapa player peduli?** — Stakes emosional, bukan hanya reward
2. **Mengapa ini sulit?** — Bukan hanya musuh yang kuat, tapi konflik nilai
3. **Apa yang berubah?** — Dunia, karakter, atau player-perspective harus berbeda setelahnya

---

## 📋 Quest Template

```markdown
## QUEST: [QUEST ID] — [Quest Name]

**Type:** [Main / Side / Hidden / Faction / Character]
**Act:** [Act 1 / 2A / 2B / 3]
**Giver:** [Who gives this quest — and why THEY need it done]
**Location:** [Starting location]
**Estimated Playtime:** [Short 5-10m / Medium 15-30m / Long 45m+]

---

### 🎯 Quest Hook
> The moment that makes the player WANT to do this quest.
> This is NOT the objective — this is the emotional entry point.

[Write 2-3 sentences: What does the player see, hear, or discover that makes this feel urgent or intriguing?]

---

### 📖 Quest Premise
**Surface Goal:** [What it looks like on the quest log — "Find the missing merchant"]
**Real Story:** [What it's actually about — "A father made a terrible deal to save his son"]
**Thematic Question:** [The moral/philosophical question this quest raises]

---

### 🗺️ Quest Structure

#### Phase 1 — SETUP
**Objective:** [Clear, specific action]
**Location:** [Where]
**Narrative Beat:** [What story moment happens here]
**Player Discovery:** [What they learn / find / witness]
**Emotional Target:** [Curiosity / Unease / Hope / Dread]

#### Phase 2 — COMPLICATION
**Trigger:** [What reveals the complication]
**New Objective:** [How the quest shifts]
**The Twist/Reveal:** [Something is not what it seemed]
**Player Choice (if any):** [Any decision point here]
**Emotional Target:** [Tension / Conflict / Empathy / Surprise]

#### Phase 3 — CLIMAX
**Final Objective:** [The decisive action]
**Stakes:** [What happens if player fails / makes wrong choice]
**Major Choice (if applicable):** [The moral crux of the quest]
**Emotional Target:** [Dread / Defiance / Grief / Triumph]

#### Phase 4 — RESOLUTION
**Outcome A:** [If player chose / did X]
**Outcome B:** [If player chose / did Y]
**World Change:** [What is visibly different in the world now]
**Character Change:** [How NPC(s) have changed]
**Echo Forward:** [How this quest matters later in the story]

---

### 🧩 Quest Objectives (Player-Facing)

```
PRIMARY
☐ [Objective 1 — clear, actionable]
☐ [Objective 2]
☐ [Objective 3 — often the twist]

OPTIONAL
☐ [Optional 1 — rewards curiosity or thorough players]
☐ [Optional 2 — reveals lore or character depth]

HIDDEN (revealed mid-quest)
☐ [Hidden objective — emerges from player discovery]
```

---

### 💬 Key Dialogue Moments

**Quest Opening (Hook dialogue):**
> [2-4 lines of NPC dialogue that establishes hook — use subtext]

**Mid-Quest Revelation:**
> [The moment the quest becomes about something deeper]

**Final Choice Prompt (if applicable):**
> [The question or ultimatum that forces player to decide]

**Quest Completion:**
> [What the NPC says — changed by player choices]

---

### 🌿 Branch Points

| Branch ID | Trigger | Option A | Option B | Consequence |
|-----------|---------|----------|----------|-------------|
| Q[ID]-B1 | [When] | [Choice A] | [Choice B] | [How it changes outcome] |

---

### 🎁 Rewards

**Catatan Penting:** Untuk saat ini, reward quest dibatasi hanya pada tiga jenis: **Exp**, **Gold**, dan **Item**. Jenis reward lain (mis. unlocks, mata uang selain Gold, perks unik) akan ditambahkan di masa mendatang setelah arahan desain lebih lanjut.

**Narrative Rewards (PALING PENTING):**
- [What story knowledge / relationship / world understanding is gained]

**Mechanical Rewards (hanya yang diizinkan):**
- Exp: [Amount — jelaskan skala/kenaikan atau rentang yang wajar]
- Gold: [Amount — gunakan `Gold` sebagai mata uang standar untuk reward quest]
- Item: [Deskripsi item — jelaskan fungsi dan alasan tematisnya]

Semua reward harus tematik dan memiliki justifikasi naratif: pilih jumlah `Exp`/`Gold` atau jenis `Item` yang masuk akal untuk konteks quest dan tidak merusak keseimbangan progression.

**Relationship Impact:**
- [NPC Name]: [+/-] [Why]
- [Faction Name]: [+/-] [Why]

---

### 🔗 Quest Connections

**Prerequisites:** [What must be done before this unlocks]
**Unlocks:** [What becomes available after completion]
**Conflicts With:** [Quests that become unavailable if this is done]
**References:** [Other quests this quest acknowledges or builds on]

---

### 📌 Design Notes

**What makes this quest memorable:**
[The ONE thing players will remember — the emotional image, the impossible choice, the unexpected reveal]

**Continuity Flags:**
```yaml
flags_set_on_complete:
  - quest_[id]_complete: true
  - [specific_outcome_flag]: [value]
relationship_changes:
  - npc_[name]_trust: [+/-value]
world_state_changes:
  - [location/situation]: [new state]
```
```

---

## 🏗️ Quest Type Reference

### 🔴 Main Quest
- Drives the **central narrative forward**
- Always has **multiple meaningful outcomes**
- Must reference **at least one side quest** thread if possible
- Player should feel: *"This changed everything"*

### 🟡 Side Quest
- Enriches the **world and its people**
- Reveals **lore through personal story** (not exposition)
- Can be completed in any order — must be **self-contained**
- Player should feel: *"I'm glad I stopped to do this"*

### 🟢 Character Quest
- Deepens a **companion or important NPC**
- Reveals their **Want / Need / Fear / Wound** (from `characters.instructions.md`)
- Completion meaningfully shifts the **relationship dynamic**
- Player should feel: *"I finally understand who they really are"*

### 🔵 Faction Quest
- Advances **faction standing** with real world consequences
- Completing one **costs something** with another faction
- Reveals **faction's true nature** — not just their propaganda
- Player should feel: *"Every side has a cost"*

### 🟣 Hidden Quest
- Discovered through **exploration or curiosity**, not map markers
- Rewards **attentive players** with exceptional story content
- Often reveals **deep lore** or **alternative perspective** on main events
- Player should feel: *"Not everyone was meant to find this"*

---

## ⚙️ Quest Pacing Rules

### The Three-Beat Rule
Every quest, no matter how short, must have:
```
HOOK → COMPLICATION → PAYOFF
```
Even a 5-minute fetch quest can have all three if designed well.

### Avoid These Quest Sins ❌

| Sin | Example | Fix |
|-----|---------|-----|
| **The Pure Fetch** | "Get 10 wolf pelts" | Add a reason. Add a character. Add a consequence. |
| **The Invisible NPC** | Quest giver has no personality | Give them a conflict, not just a job |
| **The Hollow Choice** | Binary good/evil with no nuance | Make both options have real trade-offs |
| **The Silent Consequence** | Player choices ignored afterward | Add echo moments, NPC reactions, world changes |
| **The Orphan Quest** | No connection to anything else | Thread it into the world — reference it later |
| **The Exposition Delivery** | Quest exists just to tell lore | Lore must emerge from conflict, not lectures |

### Layering Complexity
```
Simple quest surface:     "Find the missing girl"
Hidden layer 1:           The girl doesn't want to be found
Hidden layer 2:           Her family is the reason she ran
Hidden layer 3:           She found something dangerous — and she's protecting everyone by hiding
Player realization:       "This quest was never about finding her. It was about deserving her trust."
```

---

## 🗃️ Quest Registry

> Track all quests here to manage dependencies and flag conflicts.

```yaml
quests:
  - id: "Q001"
    name: ""
    type: "main"
    status: "planned"       # planned / in-progress / complete / locked
    act: "ACT 1"
    prerequisites: []
    unlocks: []
    conflicts_with: []
    flags_set: []
    
  - id: "Q002"
    name: ""
    type: "side"
    status: "planned"
    act: "ACT 1"
    prerequisites: []
    unlocks: []
    conflicts_with: []
    flags_set: []
```

---

## 🎖️ Quest Quality Checklist

Before finalizing any quest:

**Story**
- [ ] Does the quest have a **surface goal** AND a **real story**?
- [ ] Is there an **emotional hook** within the first 60 seconds?
- [ ] Does the quest have a **complication** that changes what it's about?
- [ ] Is there at least **one meaningful choice**?
- [ ] Does something **meaningfully change** by the end?

**Characters**
- [ ] Is the quest giver a **person**, not just a function?
- [ ] Do NPCs **react differently** based on player choices?
- [ ] Is there at least **one character moment** that reveals depth?

**World**
- [ ] Does the quest reveal something about **how this world works**?
- [ ] Is the quest **rooted in this world's specific conflicts** (not generic)?
- [ ] Does completing it **change something visible** in the world?

**Mechanical**
- [ ] Are objectives **clear and specific**?
- [ ] Are optional objectives **genuinely optional** (not required to understand the story)?
- [ ] Are rewards **thematically appropriate** (not arbitrary)?
- [ ] Are **flags and variables** documented for continuity?

**Connections**
- [ ] Does this quest **reference** or **echo** other quests?
- [ ] Is there an **echo forward** — will this matter later?
- [ ] Are conflicts with other quests **documented**?
