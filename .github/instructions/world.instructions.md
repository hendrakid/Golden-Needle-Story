---
applyTo: "**/*.lore.md, **/world/**, **/lore/**, **/codex/**"
---

# 🌍 World Building Instructions

Maintain the consistency, depth, and internal logic of the game world.

---

## 🗺️ World Overview Template

```markdown
## World Name: [TBD]

**Genre:** [Fantasy / Sci-Fi / Post-Apocalyptic / Horror / etc.]
**Tone:** [Grimdark / Epic / Hopeful / Bittersweet / etc.]
**Scale:** [Local / Continental / Planetary / Multiversal]
**Time Period:** [Ancient / Medieval / Industrial / Modern / Future]
**Central Conflict:** [The core tension driving this world's history]
```

---

## 📜 The World Bible

### Prime Directives of This World
> These are the **unbreakable rules** of how this world works. Copilot must NEVER violate these.

```
1. [Core Rule 1 — e.g., "Magic has equal cost to benefit"]
2. [Core Rule 2 — e.g., "The dead cannot be truly revived"]
3. [Core Rule 3 — e.g., "Technology and nature are at war"]
```

### How This World Differs From Reality
List the **key departures** from our world:
- [ ] Different physics rules?
- [ ] Different social structures?
- [ ] Magic/technology systems?
- [ ] Different history?
- [ ] Non-human sentient species?

---

## 🏛️ Factions & Powers

### Faction Template
```markdown
### [FACTION NAME]

**Alignment:** [Not necessarily good/evil — what do they VALUE?]
**Motivation:** What does this faction want?
**Method:** How do they pursue it?
**Strength:** What makes them powerful?
**Weakness:** What makes them vulnerable?
**Relationship to Player:** [Potential ally / enemy / neutral / complex]

**How Members Talk:**
- Vocabulary examples
- Common phrases or slogans
- What they never say / avoid
```

---

## 🌐 Geography & Locations

### Location Entry Template
```markdown
### [LOCATION NAME]

**Type:** [City / Dungeon / Wilderness / Ruin / etc.]
**Region:** [Where in the world]
**Atmosphere:** [The feeling of being here]
**History:** [What happened here — briefly]
**Current State:** [Active / Abandoned / Contested / Neutral]
**Notable Features:** [What makes this place visually/narratively distinct]
**Story Function:** [What narrative purpose does this place serve]

**Sensory Details:**
- Sight: 
- Sound: 
- Smell: 
- Touch/Feel: 
```

---

## ⚙️ Systems & Rules

### Magic / Technology System
> Define how the **central power system** works with precision. Vague systems break stories.

```markdown
**System Name:** [e.g., "The Resonance" / "Nano-synthesis" / "Blood Contracts"]

**Source:** Where does it come from?
**Mechanism:** How does it work?
**Cost:** What does it require / take from the user?
**Limits:** What can it NOT do? (Limits make it interesting)
**Cultural View:** How does society see it? Feared? Revered? Regulated?
**Visual Signature:** What does it look like when used?
**Narrative Function:** How does it drive conflict?
```

### Economy & Resources
- What do people need to survive?
- What is scarce and therefore valuable?
- Who controls resources and why?
- How does economic pressure affect the story?

---

## 📚 Lore Delivery Methods

### Show World Through Story, Not Lecture

**Instead of:** *"The Accord of Ashenveil was signed 400 years ago establishing the laws of magic..."*

**Use:**
- A character cursing under their breath using old Accord terminology
- A broken statue with an inscription half-worn away
- An NPC who acts paranoid about mentioning magic near officials
- Environmental storytelling: scorched earth, strange symbols, conflicting murals

### Lore Delivery Hierarchy (Best to Worst)
1. **Environmental storytelling** — player discovers it visually
2. **Action/consequence** — world rules are demonstrated, not explained
3. **Character behavior** — culture shown through how people act
4. **Organic dialogue** — information emerges from conversation naturally
5. **Optional codex/journal** — detailed lore for those who want it
6. **NPC exposition** — used sparingly, only when other methods fail

---

## 🔍 World Consistency Rules

### Before Adding Any World Element, Ask:
1. Does this fit the **established tone** and **genre**?
2. Does this follow the **prime directives** (unbreakable world rules)?
3. Does this create **interesting conflict** or just fill space?
4. Can this be **shown** rather than explained?
5. Does this open **story possibilities** rather than close them?

### Retcon Protocol
If a world element needs to change:
- Document what changed and why
- Update all affected lore entries
- Add a note to `progress.instructions.md`
- Check `characters.instructions.md` for affected characters

---

## 🗃️ Active Lore Registry

> Track all established world facts here to prevent contradictions.

```yaml
confirmed_facts:
  - fact: ""
    source_scene: ""
    date_added: ""

contradictions_to_avoid:
  - ""

mystery_boxes_planted:
  - mystery: ""
    planted_in: ""
    resolution_planned: ""
```
