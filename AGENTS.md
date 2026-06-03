# AGENTS.md

## Website Scope

This repository is the static GitHub Pages website for `River & Palace`
marketing and coming-soon content.

- Keep the site static unless the user explicitly asks for a framework, build
  step, package manager, analytics, or deployment automation.
- Do not add external asset dependencies, tracking scripts, or third-party
  embeds without explicit approval.
- Do not make app release, App Store availability, pricing, multiplayer,
  tournament, social, ranking, or online-service claims unless the main product
  repo currently supports that wording.
- Keep this website English-first. Chinese text is allowed where it reflects
  active product glyphs, board labels, or asset provenance.
- Keep local preview instructions aligned with `README.md`.

## Main Repo Source Of Truth

Before changing website copy, visuals, feature descriptions, or copied assets,
check the active product repo at:

```text
/Users/jonh/Development/river-and-palace
```

Use that repo as the source of truth for the following areas.

### Chinese Text

- Use exact in-app piece glyphs from
  `/Users/jonh/Development/river-and-palace/apple/Sources/RiverPalaceApple/FacadeFormatting.swift`
  and
  `/Users/jonh/Development/river-and-palace/apple/Sources/RiverPalaceApple/PieceCheatsheetView.swift`.
- Do not invent alternate glyph mappings, simplified/traditional substitutions,
  pinyin spellings, or English piece names for website copy.
- For board river labels, use the documented `楚河` / `漢界` treatment from
  `/Users/jonh/Development/river-and-palace/assets/source/ios_board_art/README.md`.
- Preserve the product's English-first positioning in user-facing marketing
  copy.

### Visual Styles

- Match the active app brand palette, textures, and chrome from
  `/Users/jonh/Development/river-and-palace/apple/Sources/RiverPalaceApple/BrandStyle.swift`
  and the current SwiftUI app surfaces.
- Prefer active runtime assets and source-asset documentation from the main repo
  over new visual directions.
- Do not introduce user-selectable theme language or a different visual system
  unless the main repo's product guardrails change.
- If copying, deriving, regenerating, or replacing website assets, update
  `ASSET_PROVENANCE.md` in the same change with the source path and derivation
  notes.

### Available Features

- Verify available and planned feature claims against
  `/Users/jonh/Development/river-and-palace/README.md` and
  `/Users/jonh/Development/river-and-palace/TODO.md` before editing website
  copy.
- Current implemented iOS claims may mention Classic Xiangqi human-vs-AI with
  the project-owned local AI, Shadow Mode, Board Reveal/Jieqi, replay and
  restart flows, resign handling, check/checkmate/result presentation, the
  in-game mode menu, and adaptive iPhone/iPad layouts.
- Research or planned items must be described as research, planned, or future
  work. This includes service-backed Pikafish play, multiplayer, adjustable AI
  difficulty, dark/reveal puzzle modes, replay analysis, and training flows.
- Avoid stale or overstated claims such as "latest strong AI" unless the main
  repo currently supports that exact claim.

## Workflow Guardrails

- Run `git status --short` before editing. Preserve unrelated dirty files and
  do not revert user changes.
- The AWS CLI is available. Use `--profile river-and-palace-admin` for all AWS
  CLI commands, and verify the caller identity with
  `aws sts get-caller-identity --profile river-and-palace-admin` before
  account-backed work.
- Keep routine website changes narrowly scoped to `index.html`, `styles.css`,
  `README.md`, `ASSET_PROVENANCE.md`, or copied assets only when the task
  requires them.
- Do not change `CNAME`, GitHub Pages settings, custom-domain behavior, or DNS
  guidance unless explicitly requested.
- For docs-only changes, `git diff --check` plus a final `git status --short`
  is sufficient verification.
- For visual or layout changes, preview the static site locally and check
  relevant desktop and mobile widths before finishing.
