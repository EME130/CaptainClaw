# OpenClaw Roadmap

A game is not just computation — it's computation with time, state, and interaction.

OpenClaw is a C++ reimplementation of Captain Claw (1997), built from scratch. This roadmap charts the path from where we are today to where we believe this project can go: **running on every Von Neumann machine that matters, accessible to every player who wants to play.**

Two tracks run in parallel. Platform reach and accessibility are not sequential — they grow together.

---

## Platform Track

### P1 — Solidify Existing Platforms

The foundation. Before we go wider, we go deeper.

- [ ] Modernize CI/CD pipeline (replace Travis CI, add GitHub Actions for all targets)
- [ ] CMake build system cleanup and standardization
- [ ] Windows: update VS project support, test on modern toolchains
- [ ] macOS: native .app bundle, Homebrew formula
- [ ] Linux: Flatpak / AppImage distribution
- [ ] Android: complete deployment pipeline, Play Store readiness
- [ ] Emscripten: fix MIDI playback, death/teleport fade effects, browser quirks

### P2 — New Platforms

Go where the players are — and where they will be.

- [ ] **iOS** — touch control adaptation, Metal rendering path, App Store packaging
- [ ] **ARM Linux** — Raspberry Pi, Steam Deck (native), embedded boards
- [ ] **Console homebrew** — Switch homebrew, Vita, community-driven ports

### P3 — The Hardware Horizon

The game loop is fundamentally imperative and sequential. Even massively parallel systems need a Von Neumann CPU to orchestrate the game — the GPU just handles what's naturally parallel. But what if the game *is* the hardware?

- [ ] FPGA feasibility study — analyze game logic for hardware reimplementation
- [ ] MiSTer core development — bring Captain Claw to dedicated retro hardware
- [ ] HDL reimplementation of core game systems (state machine, physics, rendering pipeline)
- [ ] Hardware-software co-design documentation for the community

---

## Accessibility Track

Every platform we support should be playable by everyone. Accessibility is not a feature — it's a commitment.

### A1 — Foundation

The scaffolding that everything else builds on.

- [ ] Accessibility abstraction layer (platform-agnostic API for assistive features)
- [ ] Fully remappable controls (keyboard, gamepad, touch)
- [ ] Subtitle and caption system for all dialogue and audio cues
- [ ] High contrast mode
- [ ] Colorblind palette options (protanopia, deuteranopia, tritanopia)
- [ ] Adjustable text size across all UI

### A2 — Platform-Native Integration

Meet players where their OS already helps them.

- [ ] **macOS / iOS** — VoiceOver support for menus and HUD
- [ ] **Android** — TalkBack integration
- [ ] **Windows** — Narrator and UI Automation support
- [ ] **Web** — ARIA roles and semantic HTML for Emscripten UI overlay
- [ ] Screen reader-navigable menus on all platforms
- [ ] Audio cues and spatial audio descriptions for visual gameplay events

### A3 — Comprehensive

The last mile — and the hardest.

- [ ] Cognitive accessibility: adjustable game speed, simplified UI mode, clear waypoints
- [ ] One-handed play mode (full game completable)
- [ ] Switch device and adaptive controller support
- [ ] Motor accessibility profiles (presets for common needs)
- [ ] Community accessibility audit and playtesting program
- [ ] Accessibility documentation and contribution guide

---

## How to Contribute

Every milestone has open work. Pick what calls to you:

| Interest | Start here |
|---|---|
| Build systems & CI | P1 |
| Mobile development | P2 (iOS, Android) |
| Low-level / embedded | P3 (FPGA, ARM) |
| UI/UX engineering | A1, A2 |
| Assistive technology | A2, A3 |
| Playtesting | A3 |

Open an issue, pitch an idea, or just send a PR. No contribution is too small.

---

<br>

<p align="center"><sub>

*Some of us look at a game and see what it is. Others see what it could become — not just one game, but the idea that any game worth remembering is worth reimagining. If you've ever stared at a title screen and thought "this deserves to live again, everywhere, for everyone" ... well. We should talk. The door is open. The project doesn't have a name yet. Or maybe it does.*

</sub></p>
