# FC Pixel README Optimization Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Rebuild the profile README into a technical-credibility-first FC pixel layout with richer dynamic icons and controlled visual density.

**Architecture:** Keep `README.md` as the single source of profile layout, with local assets providing style-defining visuals and external widgets providing live engineering/activity signals. Structure sections as Hero -> Credibility -> Inventory -> Now Building -> Activity.

**Tech Stack:** GitHub Profile README Markdown, inline HTML, local PNG/GIF assets, shields.io, readme-typing-svg, github-readme-stats, contribution snake, activity graph.

---

### Task 1: Prepare Dynamic Local Assets

**Files:**
- Create: `assets/hero-loop.gif`
- Create: `assets/pixel-chip.gif`
- Create: `assets/pixel-guitar.gif`
- Verify: `assets/image.png`
- Verify: `assets/guitar_cutout_trimmed.png`

**Step 1: List current asset inventory**

Run: `Get-ChildItem assets -File | Select-Object Name,Length`  
Expected: existing static assets are visible and valid.

**Step 2: Create or import hero animation**

Run: `# add hero-loop.gif into assets/`  
Expected: `assets/hero-loop.gif` exists and can render.

**Step 3: Create or import two small supporting animations**

Run: `# add pixel-chip.gif and pixel-guitar.gif into assets/`  
Expected: both files exist under `assets/`.

**Step 4: Verify all planned local media paths**

Run: `rg -n "hero-loop|pixel-chip|pixel-guitar|image\\.png|guitar_cutout_trimmed\\.png" README.md assets`  
Expected: filenames are consistent with intended references.

**Step 5: Commit asset-only changes**

```bash
git add assets/hero-loop.gif assets/pixel-chip.gif assets/pixel-guitar.gif
git commit -m "feat: add fc pixel animated assets for profile readme"
```

### Task 2: Rebuild Hero and Credibility Sections

**Files:**
- Modify: `README.md`

**Step 1: Rewrite Hero block structure**

Run: `# replace top visual block in README.md with hero animation + one-line identity copy`  
Expected: Hero includes local animated anchor and concise role statement.

**Step 2: Keep typing animation but tune lines for engineering focus**

Run: `# update readme-typing-svg lines in README.md`  
Expected: text emphasizes embedded engineering and build momentum.

**Step 3: Place credibility modules immediately after Hero**

Run: `# ensure stats and top-langs stay in Tech Credibility section`  
Expected: technical proof appears before personality-heavy modules.

**Step 4: Validate markdown fence/tag balance**

Run: `Get-Content -Raw README.md`  
Expected: no broken markdown fences and no malformed HTML tags.

**Step 5: Commit hero/credibility refactor**

```bash
git add README.md
git commit -m "refactor: reorganize hero and technical credibility sections"
```

### Task 3: Add Inventory and Now Building Sections

**Files:**
- Modify: `README.md`

**Step 1: Convert inventory into compact pixel-style rows**

Run: `# adjust Inventory block to stack/core/tool/interest rows`  
Expected: cleaner rows with reduced visual noise and preserved pixel mood.

**Step 2: Add Now Building module with 3 short progress lines**

Run: `# insert Now Building section under Inventory`  
Expected: three bullets only: current, near-term goal, next step.

**Step 3: Attach small local animated icons in Now Building**

Run: `# reference assets/pixel-chip.gif and assets/pixel-guitar.gif`  
Expected: motion supports status visibility without dominating layout.

**Step 4: Keep About Me code snippet concise**

Run: `# trim About Me code block to 6-10 lines`  
Expected: maintains identity signature while reducing scroll length.

**Step 5: Commit mid-page information architecture update**

```bash
git add README.md
git commit -m "feat: add pixel inventory and now-building modules"
```

### Task 4: Final Layout and Link Verification

**Files:**
- Modify: `README.md` (if fixes required)

**Step 1: Verify all local image references resolve**

Run: `rg -n "assets/" README.md`  
Expected: all referenced files exist in `assets/`.

**Step 2: Verify no obsolete image path remains**

Run: `rg -n "khalil_pixel|embedded_engineer_pixel" README.md`  
Expected: no stale paths unless intentionally retained.

**Step 3: Inspect final diff**

Run: `git diff -- README.md`  
Expected: section order and content match approved FC Pixel v3 design.

**Step 4: Perform readability pass**

Run: `# markdown preview check in IDE`  
Expected: no crowded first screen, spacing is balanced between icons.

**Step 5: Final commit**

```bash
git add README.md
git commit -m "style: optimize profile readme for fc pixel dynamic layout"
```

