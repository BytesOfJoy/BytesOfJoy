# Profile README Refresh Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Redesign profile README into a personal-brand-first cyber pixel style with dark neon theme and simplified modules.

**Architecture:** Keep the profile README as a single markdown artifact with embedded HTML blocks and badge/image services. Use one dominant visual flow: Hero -> Identity -> Stack -> Stats -> Snake -> Signature code block.

**Tech Stack:** GitHub Profile README Markdown, inline HTML, shields.io badges, github-readme-stats, contribution snake output.

---

### Task 1: Rewrite README Content and Visual Modules

**Files:**
- Modify: `README.md`
- Verify: `README.md` render via markdown preview

**Step 1: Write target structure checklist**

```text
Hero, Player Card, Bright Strip, Equipment, Stats, Snake, Signature Code Block
```

**Step 2: Replace existing sections with new dark-neon mixed-language copy**

```markdown
Use centered hero + avatar + mixed CN/EN copy + neon badges.
```

**Step 3: Keep only selected modules**

```markdown
Keep GitHub Stats and Snake.
Remove Top Langs and Activity Graph.
```

**Step 4: Verify formatting**

Run: `Get-Content -Raw README.md`  
Expected: All sections present, no broken markdown fences, no removed asset path errors.

**Step 5: Review diff**

Run: `git -C F:/Project/Github/BytesOfJoy diff -- README.md`  
Expected: A full README redesign aligned with approved direction.
