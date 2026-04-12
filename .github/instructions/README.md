# Instruction Files — Maintenance Guide

This folder contains specialized instruction files that guide Copilot's behavior when working with different aspects of the game story.

---

## 📂 Instruction Files Overview

| File | Applies To | Purpose |
|------|-----------|---------|
| [branching.instructions.md](branching.instructions.md) | `**/*.branch.md`, branches/, choices/ | Choice & consequence system design |
| [characters.instructions.md](characters.instructions.md) | `**/*.character.md`, characters/, dialogue/ | Character profiles & voice consistency |
| [dialogue.instructions.md](dialogue.instructions.md) | `**/*.dialogue.md`, dialogue/ | Dialogue writing standards & techniques |
| [pacing.instructions.md](pacing.instructions.md) | `**/*.scene.md`, scenes/, acts/ | Narrative pacing & tension control |
| [progress.instructions.md](progress.instructions.md) | `**/*.story.md`, story/, narrative/, scenes/ | Story arc tracking & progress |
| [quest.instructions.md](quest.instructions.md) | `**/*.quest.md`, quests/ | Quest design philosophy & templates |
| [tone.instructions.md](tone.instructions.md) | story/**, scene/dialogue/quest/character files | Tone, mood & prose style guide |
| [world.instructions.md](world.instructions.md) | `**/*.lore.md`, world/, lore/, codex/ | World-building & lore consistency |

---

## ✅ Checklist: Adding New Instruction Files

When creating a new instruction file:

- [ ] **Valid YAML frontmatter** — Use `---` delimiters, quote `applyTo` if it contains special characters
- [ ] **Specific `applyTo` pattern** — Avoid `applyTo: "**"` unless truly applies to all files (use specific globs like `**/*.type.md` or `folder/**`)
- [ ] **Registered in index** — Add to `.github/copilot-instructions.md`:
  - List in "Project Structure Reference" section
  - Add reference in "When Helping With Story Tasks" section
- [ ] **Clear pattern matching** — Ensure target files actually match the `applyTo` glob pattern
- [ ] **Tested loading** — Open target file type and verify instruction loads correctly
- [ ] **No conflicts** — Check for contradictions with existing instructions
- [ ] **Updated this README** — Add entry to table above

---

## ✅ Checklist: After Story Elicitation Workflow

After completing elicitation and user confirms brief, verify:

- [ ] **`progress.instructions.md` updated** — Section "Current Progress Tracker" contains:
  - `world_name`, `genre`, `setting`, `tone`, `pov`, `language`
  - `story_premise` with 1-2 sentence conflict description
  - `main_characters` list with at least protagonist
  - `scenes_completed` includes `story-brief-confirmed-[date]`
  
- [ ] **Character files created** — For each main character:
  - File exists in `story/characters/[name-kebab].character.md`
  - Uses template from `characters.instructions.md`
  - Header contains `status: "draft-from-elicitation"`
  - Minimal fields filled: Name, Role, Core Identity (Want/Need/Fear)
  
- [ ] **`world.instructions.md` updated** — Section "World Overview Template" filled:
  - World Name (or TBD)
  - Genre, Tone, Scale, Time Period
  - Central Conflict
  - Prime Directives (if user mentioned world rules)
  
- [ ] **User confirmation shown** — Copilot displayed success message listing files updated

- [ ] **Context persistence tested** — In NEW conversation:
  - Request "lanjutkan cerita" or similar
  - Verify Copilot reads saved context FIRST (doesn't re-ask genre/characters)
  - Copilot says "Saya lihat ceritamu berlatar di..." using saved info

---

## 🔧 Troubleshooting

### Instruction Not Loading

**Symptom:** Opening a file doesn't load expected instruction  
**Check:**
1. Is `applyTo` pattern correct? Test with glob pattern tester
2. Is file registered in `.github/copilot-instructions.md`?
3. Is YAML frontmatter valid? Check for unquoted colons, tabs instead of spaces
4. Is the instruction file in correct folder (`.github/instructions/`)?

### Context Not Persisting Across Conversations

**Symptom:** Copilot re-asks genre/characters in new conversation  
**Check:**
1. Was elicitation workflow completed with user confirmation?
2. Do files exist: `progress.instructions.md`, `world.instructions.md`, `story/characters/*.character.md`?
3. Are those files actually updated with data (not just templates)?
4. Does `progress.instructions.md` have "Pre-Elicitation Context Check" rule?

### Multiple Instructions Conflicting

**Symptom:** Copilot receives contradictory guidance  
**Solution:**
1. Review overlapping `applyTo` patterns (some overlap is intentional, e.g., characters + dialogue)
2. Ensure instructions are complementary, not contradictory
3. Add cross-references between related instructions
4. If conflict is necessary, mark priority in instruction text

### Performance Issues (Context Window Bloat)

**Symptom:** Copilot slow, hitting context limits  
**Check:**
1. Are any instructions using `applyTo: "**"`? Narrow the pattern
2. Are instruction files too long? Consider splitting into multiple files
3. Are overlapping patterns excessive? Audit which files load together

---

## 📊 Pattern Audit

Current overlapping patterns (intentional):

- `story/dialogue/` → Loads both `characters.instructions.md` AND `dialogue.instructions.md`  
  **Why:** Dialogue requires both character voice consistency and dialogue technique guidance

- `story/acts/*/scene-*.scene.md` → Loads `pacing.instructions.md`, `progress.instructions.md`, AND `tone.instructions.md`  
  **Why:** Scenes need pacing control, story arc awareness, and tone consistency simultaneously

These overlaps are **by design** and provide comprehensive guidance for complex content types.

---

## 📝 Maintenance Schedule

**After each major story milestone:**
- Review `progress.instructions.md` — Update current act, completed scenes, active threads
- Check character files are up-to-date with story developments
- Verify world rules in `world.instructions.md` haven't been violated

**Quarterly:**
- Audit instruction file performance (which ones load together, context usage)
- Review and update examples in instructions to match current story state
- Check for outdated references or deprecated patterns

---

## 🆘 Getting Help

If instructions aren't working as expected:

1. Check this README's troubleshooting section
2. Review `.github/copilot-instructions.md` for global rules
3. Test with minimal example (create test file, verify instruction loads)
4. Check VS Code Copilot debug logs for YAML parsing errors
5. Verify file structure matches documented patterns

---

**Last Updated:** April 12, 2026  
**Maintained By:** Project Team
