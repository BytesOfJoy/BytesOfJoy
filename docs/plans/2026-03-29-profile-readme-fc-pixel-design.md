# GitHub Profile README Design (FC Pixel v3)

**Date:** 2026-03-29  
**Owner:** BytesOfJoy

## Goals
- Technical credibility first, personality expression second.
- Stronger FC/pixel identity through more dynamic icons.
- Keep readability and avoid visual clutter.

## Confirmed Decisions
- Visual direction: FC pixel theme with mixed dynamic elements.
- Dynamic strategy: mixed source.
- Core style assets are local (`assets/*.gif` / `assets/*.png`).
- Informational widgets can remain external (stats/typing/snake/activity).

## Information Architecture
1. **Hero Dynamic Zone**
   - Main local pixel animation as the visual anchor.
   - Short role statement focused on embedded engineering.
2. **Tech Credibility**
   - GitHub stats + top languages.
   - One compact badge row for core engineering stack.
3. **Pixel Inventory**
   - Pixel-style display of primary stack/tools/interests.
   - Guitar personality signal stays here (not before credibility modules).
4. **Now Building**
   - Three concise progress lines: current work, near-term objective, next step.
   - Small dynamic icon support for momentum feel.
5. **Activity**
   - Contribution snake + activity graph + view counter.

## Dynamic Asset Plan
- Local core visuals:
  - `assets/hero-loop.gif`
  - `assets/pixel-chip.gif`
  - `assets/pixel-guitar.gif`
- Existing local still images can be reused as fallback:
  - `assets/image.png`
  - `assets/guitar_cutout_trimmed.png`
- External dynamic services (auxiliary only):
  - typing SVG
  - github-readme-stats
  - contribution snake
  - activity graph

## Copy and Tone Rules
- One-line identity copy in hero; no long paragraph in first screen.
- Use consistent keywords: `Embedded`, `C++`, `Linux`, `RTOS`, `Electric Guitar`.
- Keep section titles game-themed but content engineering-first.

## Layout Rules
- Hero area max two dynamic elements.
- Limit total dynamic modules to 3-5 to control noise.
- Keep icon spacing explicit to avoid crowding.

## Acceptance Criteria
- Within 30 seconds, viewer can identify:
  - Embedded engineering orientation
  - Pixel + electric guitar personality
- First screen has clear hierarchy and no crowded overlap.
- README has no broken local image links.
- Mobile view has no obvious stacking collisions.

