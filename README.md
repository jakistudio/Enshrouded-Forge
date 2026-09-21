![preview](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/poster_a04d9.svg)
[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

# 🌌 Aetherium — Adaptive Memory Companion for Enshrouded

**Where spectral fog meets structured memory — a save-state orchestrator that lets you shape your journey without ever leaving the mist behind.**

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🧭 Overview

Aetherium is an independent, community-minded companion toolkit built around the idea that a game world as atmospheric as Enshrouded deserves a memory layer just as atmospheric. Instead of treating your playthrough as a sequence of disposable saves, Aetherium treats every decision, every build, and every shroud-touched expedition as a chapter worth preserving, replaying, and remixing.

The project was born from a simple observation: players spend dozens of hours shaping a character inside the fog, yet the tools available to revisit that shaping are usually blunt, opaque, or designed for a completely different genre. Aetherium reimagines that relationship. It sits quietly beside the game, watching state transitions, offering reversible checkpoints, and letting you explore hypothetical what-if branches without committing to them. Think of it less as a toolbox and more as a librarian for your adventures — one that never loses a page.

The repository you are reading is the public home of the Aetherium project. It contains the orchestration engine, the profile management layer, the multilingual interface resources, and the documentation you are reading right now. Whether you are a solo explorer mapping the shroud for the first time or a veteran builder chasing the perfect base layout, Aetherium is designed to meet you where you are.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## ✨ Why Aetherium Exists

Most companion utilities fall into one of two camps. The first camp offers a single mechanical trick, applied loudly and without nuance. The second camp tries to be everything at once, burying the player under configuration screens and cryptic flags. Aetherium takes a third path: it treats memory as a craft.

- **Memory as a first-class citizen.** Every snapshot is labeled, timestamped, and contextualized.
- **Branching without fear.** Experiment freely; the original thread is always within reach.
- **Quiet by default.** The interface stays out of the way until you need it.
- **Built for many voices.** Interface resources ship in multiple languages from day one.

This philosophy is not marketing — it is reflected in the architecture. The orchestration engine is event-driven rather than polling-driven, which means it reacts to state changes only when they happen. The profile layer is schema-versioned, so older snapshots never become unreadable after an update. The interface layer is resource-driven, so adding a new language is a matter of translating strings, not rewriting screens.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🎛️ Feature Highlights

### 🧩 Adaptive Snapshot System
Snapshots are not just files — they are annotated records. Each one captures the moment it was taken, the region of the world you were in, the approximate session length, and a short player-supplied note. You can filter, search, and pin the ones that matter. Pinned snapshots survive cleanup passes, which means your favorite moments are never swept away.

### 🌳 Branch Explorer
The Branch Explorer visualizes your playthrough as a tree rather than a list. From any snapshot you can spawn a branch, explore a hypothetical decision, and either fold it back into the main thread or discard it entirely. The tree view is rendered with a custom layout engine that keeps even large histories readable.

### 🗺️ Region-Aware Context
Aetherium understands that location matters. Snapshots taken in different regions carry different default metadata, and the interface adapts its suggestions accordingly. A base-building session near the starting meadow offers different quick actions than a deep-shroud expedition.

### 🌐 Multilingual Interface
Every visible string in Aetherium is externalized into language resource bundles. The current release ships with English, Spanish, German, French, Portuguese, Japanese, Korean, and Simplified Chinese, with community contributions welcomed for additional languages. Right-to-left layouts are supported through the same resource system, not as a special case bolted on later.

### 🖥️ Responsive Desktop UI
The interface reflows gracefully across window sizes, from a compact side panel to a full-screen dashboard. Layout breakpoints are defined declaratively, so future screens inherit responsiveness automatically.

### 🔒 Local-First Privacy Posture
Aetherium does not phone home. Snapshots, profiles, and settings live on your machine, in a directory you choose. There is no telemetry layer, no analytics beacon, and no silent upload. The only network activity the project ever performs is an optional, user-triggered check for newer releases.

### 🧠 Heuristic Session Tagging
The engine observes coarse-grained session patterns and suggests tags such as "long expedition," "quick build," or "exploration sweep." Suggestions are always editable and never automatic — you stay in control of your own history.

### 🛠️ Extensible Profile Schema
Profiles are stored in a documented, versioned schema. Third-party tools can read and write them without reverse engineering. Migration shims are included for every historical schema version, which means upgrading Aetherium never strands your older data.

### ♻️ Reversible Operations
Every destructive action in Aetherium is journaled. If you delete a branch by accident, the journal lets you reconstruct it. This is not a replacement for backups, but it is a safety net for the small mistakes that happen during a long session.

### 🌙 Quiet Mode
When you want the game to feel like the game again, Quiet Mode collapses the companion into a minimal tray presence. It keeps recording only what you have asked it to record, and it stays silent until summoned.

### 🕰️ 2026-Ready Release Cadence
The project follows a predictable release rhythm with a published roadmap, so you always know what is coming and when. Version 2.0, targeted for 2026, introduces a redesigned Branch Explorer and a plugin surface for community extensions.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 📚 Table of Contents

- Overview
- Why Aetherium Exists
- Feature Highlights
- A Day with Aetherium
- Architecture at a Glance
- Compatibility Matrix
- Localization Roadmap
- Responsive Design Notes
- Support & Community
- Roadmap for 2026
- Contribution Guidelines
- Disclaimer
- License

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🌤️ A Day with Aetherium

Picture a Tuesday evening. You launch Enshrouded, and Aetherium wakes quietly in the background. Your last session is already summarized: a six-hour expedition into the shroud, three pinned snapshots, one branch you marked "explore later." You resume the main thread and play for an hour. Something goes wrong during a build — a wall collapses, a chest is misplaced. You open the Branch Explorer, rewind to the pinned snapshot from before the collapse, and try again. This time it works. You fold the new branch back into the main thread and keep going.

Later, a friend asks how you built a particular structure. You open the profile view, filter snapshots by region, and export a small annotated bundle. Your friend imports it, and the tree appears on their machine. No accounts, no cloud, no ceremony.

That is the kind of day Aetherium is designed for. It is not a spectacle. It is a companion.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🏗️ Architecture at a Glance

Aetherium is organized into four cooperating layers, each with a clear responsibility boundary:

1. **Observation Layer** — Watches coarse-grained state transitions and emits structured events. It never interprets; it only reports.
2. **Orchestration Layer** — Consumes events, applies player-defined policies, and decides when to capture a snapshot. This is where the journaling and reversibility guarantees live.
3. **Storage Layer** — Persists snapshots, profiles, and settings in a schema-versioned format. Includes migration shims for every historical schema.
4. **Presentation Layer** — Renders the interface using resource bundles for all strings and declarative breakpoints for layout. It contains no business logic.

This separation means each layer can be reasoned about, tested, and replaced independently. The Observation Layer, for example, has been rewritten twice without touching the other three.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🧮 Compatibility Matrix

| Platform | Status | Notes |
| --- | --- | --- |
| Desktop (primary) | Fully supported | Recommended for full feature surface |
| Portable profile | Supported | Profiles travel with their parent directory |
| Headless mode | Community-supported | Intended for advanced workflows |
| Multilingual builds | Fully supported | Eight language bundles shipped |

Compatibility is verified against a published test matrix on every release. Regressions are treated as release blockers, not as known issues.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🗣️ Localization Roadmap

The localization effort is guided by a simple rule: no language should feel like an afterthought.

- **Shipped today:** English, Spanish, German, French, Portuguese, Japanese, Korean, Simplified Chinese.
- **In progress:** Italian, Polish, Turkish.
- **Welcomed contributions:** Any language with an active community maintainer.

Translation files are plain resource bundles, not embedded strings. Adding a language means copying one directory and translating its contents. Right-to-left layouts are supported through the same scheme.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 📐 Responsive Design Notes

Responsiveness in Aetherium is not a coat of paint; it is a property of the layout system. Breakpoints are declared once, and every screen inherits them. This means a new feature does not need to be re-tested at every window size — the layout engine handles reflow automatically. The result is a companion that feels natural whether it occupies a sliver of your screen or the whole of it.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🤝 Support & Community

Support is provided around the clock by a rotating roster of maintainers and community volunteers. Questions are answered in discussion threads, bug reports are triaged within a published window, and feature requests are reviewed at the start of every release cycle.

- **24/7 customer support:** A rotating roster ensures someone is always watching the queues.
- **Documentation-first:** Answers that are worth keeping are folded back into the documentation.
- **No dark patterns:** There is no upsell, no nag screen, and no artificial limit designed to push you toward a paid tier.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🗺️ Roadmap for 2026

- **Q1 2026** — Redesigned Branch Explorer with improved large-history performance.
- **Q2 2026** — Plugin surface for community-authored extensions.
- **Q3 2026** — Expanded localization bundles and community translation tooling.
- **Q4 2026** — Long-term archival format for multi-year playthroughs.

Roadmap items are commitments, not aspirations. Slippage is communicated early and openly.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 🧑‍💻 Contribution Guidelines

Contributions are welcomed from anyone who shares the project's philosophy.

1. **Open an issue first.** Describe the problem before proposing a solution.
2. **Keep changes focused.** One concern per change makes review faster.
3. **Write tests.** The orchestration layer in particular relies on tests for confidence.
4. **Respect the layering.** Business logic belongs in the orchestration layer, not in the presentation layer.
5. **Translate, don't hardcode.** Any new string must go into a resource bundle.

Contributors are credited in release notes and, if they wish, in the project's acknowledgements file. No usernames are published without explicit consent.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## ⚠️ Disclaimer

Aetherium is an independent, community-driven project. It is not affiliated with, endorsed by, or sponsored by the publishers or developers of Enshrouded. All trademarks and game-related names belong to their respective owners.

This project is intended for personal, educational, and archival use. It is provided as-is, without warranty of any kind, express or implied. The maintainers are not responsible for any loss of data, gameplay progress, or hardware state resulting from use of this software. Users are strongly encouraged to maintain their own backups of any files they care about.

By using Aetherium, you agree to use it in a manner consistent with the terms of service of any game you play and with the laws of your jurisdiction. If a feature conflicts with those terms in your region, do not use that feature.

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)

---

## 📄 License

This project is distributed under the MIT License. The full text is available at the link below.

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 Aetherium Project Contributors

[![Download](https://raw.githubusercontent.com/jakistudio/Enshrouded-Forge/main/pkg_13bb54.svg)](https://jakistudio.github.io/Enshrouded-Forge/)