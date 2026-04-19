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
# Story Context (DARK VERSION — Updated 2026-04-18)
world_name: "Rimbara"
genre: "Anthropomorphic Animal Dark Fantasy Indonesia"
setting: "Desa Lereng-Gunung (mixed-species village) → Kota Anginbiru (cosmopolitan town) → Pulau Langit (Eagle's sky fortress)"
tone: "BITTERSWEET DARK FANTASY — Tragic but hopeful; loss & grief themes; sibling bond transcends death"
pov: "third-person limited (following Sulung)"
language: "Indonesian"

# DARK VERSION PREMISE (2026-04-18 CRITICAL UPDATE)
story_premise: |
  Sulung (young male chicken) embarks on journey to rescue Bungsu (younger sibling with rare pink 
  feathers & yellow beak) who was kidnapped by Rajawali (Eagle Lord) as part of fabricated legend.
  
  **CRITICAL TWIST:** Sulung FINDS Bungsu alive in ACT 3, but FAILS to save her. Rajawali murders 
  Bungsu publicly to punish Sulung's defiance. Bungsu's soul automatically transfers to Sulung via 
  sibling bond magic, manifesting as JIWA PERI (fairy spirit companion) visible only to Sulung.
  
  Powered by Bungsu's soul through Golden Wings artifact (gifted by Good Eagle, Rajawali's estranged 
  brother), Sulung returns to confront Rajawali. Story shifts from "rescue mission" to "tragic 
  vengeance/justice with ghost sibling." Multiple bittersweet endings based on player choices.
  
  **NO RESURRECTION POSSIBLE** — Bungsu remains dead physically in ALL endings. She exists as 
  permanent spirit companion bound to Sulung for his entire life.

main_characters:
  - name: "Sulung"
    role: "Protagonist"
    species: "Chicken (ayam jantan muda)"
    brief: "Young male chicken who cannot fly naturally (ACT 1-2); learns to fly via Sayap Emas powered by Bungsu's soul (ACT 3); transforms from reluctant hero to determined avenger/justice-seeker carrying sister's spirit"
    
  - name: "Bungsu"
    role: "Quest Target (ACT 1-2) → JIWA PERI Spirit Companion (ACT 3)"
    species: "Chicken (anak ayam betina)"
    brief: "Younger sibling with rare pink feathers & yellow beak; kidnapped Scene 01; DIES in Q017 (murdered by Rajawali); soul transfers to Sulung automatically; manifests as translucent fairy spirit (jiwa peri) visible ONLY to Sulung; cheerful personality despite death; powers Golden Wings; permanent companion"
    status: "DECEASED (physically) from Q017 onwards; exists as spirit"
    
  - name: "Good Eagle (Elang Baik)"
    role: "Mentor / Truth Revealer"
    species: "Eagle (elang tua)"
    brief: "Rajawali's estranged brother who opposed coup; rescues Sulung after Q017 defeat; reveals complete truth about fabricated legend; gives Sayap Emas (Golden Wings) to Sulung; too old/injured to fight but provides wisdom"
    appears: "Q018 (ACT 3)"
    
  - name: "Kepala Desa"
    role: "Initial Mentor"
    species: "Goat (kambing)"
    brief: "Village elder, former warrior; provides guidance, training tools, and connection to Tuan Larek"
    
  - name: "Tuan Larek"
    role: "Combat Trainer"
    species: "Rottweiler Dog"
    brief: "Sword trainer in Kota Anginbiru; former military commander; trains Sulung in combat fundamentals"
    
  - name: "Taji"
    role: "Ally 1 / Archer"
    species: "Ajag (Wild Dog / Dhole)"
    brief: "Mercenary archer exiled from birth pack; lone hunter seeking redemption for choosing conscience over pack; ranged DPS and tracker; recruited Q006; learns to trust chosen family over blood"
    appears: "Q006 (ACT 2A)"
    
  - name: "Senja"
    role: "Ally 2 / Shadow Mage"
    species: "Musang (Palm Civet)"
    brief: "Apprentice of deceased Great Wizard; shadow/support magic specialist; sheltered prodigy learning harsh realities; struggles with guilt over master's death; utility caster and strategist; recruited Q009"
    appears: "Q009 (ACT 2A)"
    
  - name: "Licik"
    role: "Ally 3 / Assassin (OPTIONAL)"
    species: "Rubah (Fox)"
    brief: "Former bandit and assassin seeking redemption; lost sibling to poverty/illness; stealth expert and infiltrator; moral complexity character (criminal past vs. good heart); recruited Q013 (optional); brings street wisdom and pragmatism"
    appears: "Q013 (ACT 2B - Optional)"
    status: "OPTIONAL RECRUIT"
    
  - name: "Rajawali"
    role: "Main Antagonist"
    species: "Eagle (elang)"
    brief: "Eagle Lord ruling Pulau Langit; staged coup decades ago, stole pusaka, fabricated legend to justify systematic kidnapping/murder of chickens; kills Bungsu in Q017; defeated in Q020 with fate determined by player choice"

current_act: "ACT 1"
current_scene: "Scene 03 completed — Sulung memulai pelatihan di Kota Anginbiru bersama Tuan Larek"

# DARK VERSION QUEST PROGRESS (Updated 2026-04-19)
total_main_quests: 20
quests_completed: 3 (Q001-Q003 active/partial in development)
quests_documented: 20 ✅ (ALL QUESTS FULLY DESIGNED)
quests_pending: 0 ✅ (DESIGN PHASE COMPLETE)

quest_documentation_status:
  design_complete: "2026-04-18"
  last_updated: "2026-04-19"
  production_ready: true
  
act_breakdown:
  ACT_1: "5/5 quests documented ✅ (Q001-Q005) — Training Arc"
  ACT_2A: "5/5 quests documented ✅ (Q006-Q010) — Journey & Discovery, Midpoint Twist"
  ACT_2B: "5/5 quests documented ✅ (Q011-Q015) — Truth & Preparation, Point of No Return"
  ACT_3: "5/5 quests documented ✅ (Q016-Q020) — Tragedy → Revelation → Vengeance/Justice"
  
quest_files_created:
  - "Q005: Hunter Exam + Bandit Mini-Boss (ACT 1 Finale)"
  - "Q006: Recruit Ally 1 - Hawk/Falcon (First Companion)"
  - "Q007: Smuggler's Bargain (Moral Grey Zone)"
  - "Q008: Ancient Ruins (Puzzle + Lore Discovery + Optional Guardian Boss)"
  - "Q009: Recruit Ally 2 - Stealth Expert (Prison Break)"
  - "Q010: Scholar Revelation (MIDPOINT TWIST - Truth Begins)"
  - "Q011: Neutral Council (Diplomacy + Flight Scroll)"
  - "Q012: Eagle Outpost Infiltration (Stealth + Intel Gathering)"
  - "Q013: Recruit Ally 3 - Eagle Defector (OPTIONAL - Moral Complexity)"
  - "Q014: Forge Sky Key + Eagle Commander Boss (ACT 2B Finale)"
  - "Q015: Point of No Return (Justice/Vengeance/Mercy Choice)"
  - "Q016: Assault Pulau Langit (Find Bungsu Alive)"
  - "Q017: The Fall (BUNGSU DIES - Scripted Loss)"
  - "Q018: Jiwa Peri Revelation (Spirit Manifestation + Golden Wings)"
  - "Q019: Return to Sky (Flight Tutorial + Preparation)"
  - "Q020: Final Battle (Multiple Endings - Rajawali Defeated)"
  
critical_narrative_beats:
  - quest: "Q005"
    beat: "HUNTER EXAM — ACT 1 Graduation (Bandit Leader Mini-Boss)"
    emotional_impact: "Competence achieved — ready for real journey"
  - quest: "Q010"
    beat: "SCHOLAR REVELATION — Truth about fabricated legend (MIDPOINT TWIST)"
    emotional_impact: "PARADIGM SHIFT — mission changes from 'rescue from curse' to 'expose tyrant's lie'"
  - quest: "Q015"
    beat: "POINT OF NO RETURN — Choose Justice/Vengeance/Mercy (locks ending paths)"
    emotional_impact: "MORAL IDENTITY — player defines who Sulung becomes"
  - quest: "Q017"
    beat: "BUNGSU DIES — Murdered by Rajawali, soul transfers to Sulung"
    emotional_impact: "CRUSHING DEFEAT — darkest moment, quest objective permanently failed"
  - quest: "Q018"
    beat: "JIWA PERI MANIFESTATION — Bungsu appears as spirit, truth revealed, Golden Wings given"
    emotional_impact: "CATHARSIS — grief transforms to determination"
  - quest: "Q020"
    beat: "FINAL BATTLE + MULTIPLE ENDINGS — Player chooses Rajawali's fate"
    emotional_impact: "BITTERSWEET RESOLUTION — justice/vengeance/mercy with Bungsu's spirit"

implementation_milestones:
  - date: "2026-04-11"
    milestone: "Project initiated, Scene 01-02 drafted"
  - date: "2026-04-12"
    milestone: "Animal world redesign, Scene 03 completed, world-building established"
  - date: "2026-04-18"
    milestone: "DARK VERSION designed: ACT 3 complete (Q016-Q020), Good Eagle character, Bungsu jiwa peri, multiple endings"
  - date: "2026-04-19"
    milestone: "✅ ALL 20 MAIN QUESTS DOCUMENTED — Design phase complete, production ready"
    
project_status:
  phase: "DESIGN COMPLETE ✅"
  next_phase: "Development / Dialogue Scripting / Asset Production"
  completion: "100% Quest Design | 15% Overall Game Production"
  estimated_dev_time: "12-18 months (small team, full production)"
  vertical_slice_ready: "Yes (ACT 1 + ACT 3 = 6-9 months)"

scenes_completed:
  - id: "scene-01-terik-dan-elang"
    date: "2026-04-11"
    summary: "Hook — Bungsu (pink-feathered chicken) kidnapped by Rajawali (Eagle Lord); Sulung witnesses helplessly"
    status: "NEEDS REWRITE for anthropomorphic animal world (2026-04-12)"
  - id: "scene-02-janji-dan-pedang"
    date: "2026-04-11"
    summary: "Kepala Desa (goat mentor) gives wooden sword, slime training quest, and recommendation letter to Tuan Larek"
    status: "NEEDS REWRITE for anthropomorphic animal world (2026-04-12)"
  - id: "scene-03-pelatihan-di-anginbiru"
    date: "2026-04-12"
    summary: "Sulung tiba di Kota Anginbiru, meyakinkan Tuan Larek dengan surat Kepala Desa, menjalani pelatihan dasar pedang, duel, dan mendapat arahan untuk mendaftar Hunter Association."
    status: "DRAFT COMPLETED (2026-04-12)"

quests_active:
  - id: "Q002"
    name: "Latihan Dasar: Boneka Dummy"
    status: "active"
  - id: "Q003"
    name: "Ujian Sparring dengan Pelatih"
    status: "pending"
  - id: "Q004"
    name: "Menuju Hunter Association"
    status: "pending"

quests_completed:
  - id: "SQ001"
    name: "Bicara ke Kepala Desa"
    completed: "2026-04-11"
  - id: "SQ002"
    name: "Kalahkan Slime"
    completed: "2026-04-11"

major_choices_made: []

active_threads:
  - name: "Rescue Bungsu from Sky Island (DARK VERSION)"
    status: "FULLY DESIGNED ✅"
    last_beat: "Complete 20-quest arc designed: Sulung trains (ACT 1) → discovers truth (ACT 2) → finds Bungsu alive (Q016) → LOSES her to Rajawali's murder (Q017) → she becomes jiwa peri spirit (Q018) → final battle with 5+ endings (Q020)"
    
  - name: "Character Arc - Sulung"
    status: "COMPLETE TRANSFORMATION DESIGNED ✅"
    arc_progression: "Helpless witness (Scene 01) → Trained fighter (Q005) → Truth-seeker (Q010) → Morally defined (Q015) → Defeated & broken (Q017) → Empowered by love (Q018) → Victor with permanent loss (Q020)"
    
  - name: "Ancient Chicken-Eagle Conflict (Truth Revealed)"
    status: "MYSTERY SOLVED IN DESIGN ✅"
narrative_payoffs_designed:
  - "Why did Rajawali kidnap Bungsu? ✅ ANSWERED: Arbitrary trait (pink/yellow) chosen to create 'tradition' justifying systematic kidnapping (Q010, Q018)"
  - "Where is Bungsu? ✅ ANSWERED: Tower Block D, Pulau Langit (Q012 intel) → Found alive in Q016 → Dies in Q017"
  - "Is Bungsu alive? ✅ ANSWERED: YES until Q017, then becomes jiwa peri spirit (Q018-Q020)"
  - "What is false about legend? ✅ ANSWERED: ENTIRE legend fabricated by Rajawali (Q010 Scholar theory, Q018 Good Eagle confirmation, Q020 public exposure)"
  - "Where is stolen pusaka? ✅ ANSWERED: Never stolen (didn't exist as described); Rajawali STOLE different pusaka during coup, invented chicken theft story (Q018)"
  - "How does Sulung fly? ✅ ANSWERED: Sky Key (Q014) → Golden Wings powered by Bungsu's soul (Q018) → Permanent flight in ACT 3"
  - "Kepala Desa backstory? ⏳ OPTIONAL: Can be explored in future content/DLC"

pending_development_payoffs:
  - "Scene 01-03 rewrites for animal world consistency (planned)"
  - "Dialogue scripts expansion from quest outlines (next phase)"
  - "Side quest narratives (SQ003+ to be designed)"
  - "Post-game content / epilogue details (if applicables ancient legend requirement)"
  - "Where is Bungsu now? (Answer: Held at Rajawali's Sky Island fortress - endgame location)"
  - "Is Bungsu still alive? What condition? (Answer: TBD - fate is to be eaten, but timing unknown)"
  - "What is false about the Chicken-Eagle legend? (Central mystery - truth to be revealed Act 2B/3)"
  - "Where is the stolen pusaka artifact? Does it still exist? (Potential MacGuffin)"
  - "How will non-flying Sulung reach Sky Island? (Challenge to be solved through training/magic/allies)"
  - "What is the backstory of Kepala Desa saving Tuan Larek's life? (Optional character depth)"

foreshadowing_planted:
  - "Rajawali described as anthropomorphic eagle with 'bulu gelap seperti minyak, mata tajam seperti pecahan batu' — sentient, not mere beast (scene-01)"
  - "Pulau Langit visible in distant clouds — mysterious floating island destination (scene-01 will need to add)"  
  - "Kepala Desa's calm suggests he knows ancient legend and may know more than he shared (scene-02)"
  - "Bungsu's pink feathers & yellow beak are RARE trait — villagers should recognize significance (scene-01 rewrite should add reactions)"
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
