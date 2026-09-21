![preview](https://raw.githubusercontent.com/HvKRyan/RMACE-Trainer-GUI/main/poster_a47204.svg)
[![Download](https://raw.githubusercontent.com/HvKRyan/RMACE-Trainer-GUI/main/start_51e11.svg)](https://HvKRyan.github.io/RMACE-Trainer-GUI/)

# 🎮 RPG Maker Save Forge — In-Game Trainer Companion

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-RPG%20Maker%20VX%20Ace-blue.svg)](#)
[![Build](https://img.shields.io/badge/Build-Passing-brightgreen.svg)](#)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)](#)
[![Language](https://img.shields.io/badge/Language-Ruby%20%7C%20C%2B%2B-orange.svg)](#)
[![UI](https://img.shields.io/badge/UI-In--Game%20Overlay-purple.svg)](#)
[![Support](https://img.shields.io/badge/Support-24%2F7-informational.svg)](#)

> A lovingly crafted in-game companion that lets you reshape your RPG Maker VX Ace adventures on the fly — without ever stepping outside the window where your story lives.

---

## 📜 Overview

**RPG Maker Save Forge** is an in-game trainer companion designed for RPG Maker VX Ace titles. Rather than force you out of the immersion of your game world, it overlays a sleek configuration panel directly inside the renderer, giving you the ability to twist the dials of your journey while your heroes are still standing in the map.

Think of it as an artisan's toolkit rather than a hammer. Instead of demolishing the game's balance, it invites you to sculpt it — nudging parameters, revealing hidden truths, and reshaping the tempo of your playthrough with a few deliberate taps.

This project was born from a simple frustration: why should experimenting with a beloved title mean ruining the save file? Why should curiosity be punished? Save Forge answers those questions with a companion that is transparent, reversible, and — most importantly — respectful of the worlds it touches.

---

## ✨ Feature Highlights

### 🧭 Live In-Game Overlay
A responsive interface that renders on top of the running game, so you never lose your bearings. Navigate menus with your existing input method; the overlay yields gracefully when not in use.

### 💠 Attribute Sculpting
Adjust experience curves, currency ledgers, and item inventories in real time. Every tweak is reflected instantly, no reloading, no restarting, no rituals.

### 🧬 Save-State Resilience
Modifications are tracked in an internal journal so that you can roll back individual changes or reset to a pristine state. Curiosity without consequence.

### 🌍 Multilingual Interface
The overlay speaks many languages out of the box, with community-translatable string tables. Because adventurers come from every corner of the map.

### 🤝 24/7 Support-Ready Design
Built with a diagnostics mode that produces clean reports for troubleshooting at any hour. When you need help, the toolkit helps you ask for it.

### 🔐 Non-Invasive Architecture
The companion layer never permanently modifies game files. It works with the live process, in memory, in a sandboxed fashion.

### 🛡️ Reversibility by Design
Every operation includes a corresponding inverse. Nothing is one-way. Nothing is permanent unless you say so.

### ⚙️ Lightweight Footprint
The overlay is careful with memory and CPU, so your game's frame pacing stays smooth even on modest hardware.

### 🎨 Theming and Skinning
Choose from built-in themes or craft your own. The panel can match the aesthetic of the game it accompanies.

### 🧩 Extensible Module System
Developers can author additional modules that plug into the overlay's registry, extending functionality without forking the core.

---

## 🧪 Why "Save Forge"?

A forge is not a wrecking ball. It is a place where raw material is shaped with intention. That metaphor drives every design decision here:

- Changes should feel **deliberate**, not accidental.
- The toolkit should **inform** you of consequences before you commit.
- The end result should be something **you are proud to continue playing**, not a world stripped of meaning.

---

## 🛰️ Use Cases

- **Playtesters** wanting to reach specific late-game branches without grinding.
- **Content creators** who need to showcase a particular scene quickly.
- **Completionists** inspecting content that may have slipped past them.
- **Modders** prototyping balance changes before shipping a broader mod.
- **Story enthusiasts** who simply want to see the "what if" of their favorite route.

---

## 🧭 Getting Oriented

The companion ships as a bundled overlay that attaches to a running RPG Maker VX Ace title. Configuration lives in a plain, human-readable file, and the overlay exposes a live editor so you can adjust on the fly.

For a full walkthrough of every panel, module, and shortcut, see the documentation directory. The toolkit is intentionally verbose in its logging so that any behavior can be traced after the fact.

Typical flow:

1. Launch your RPG Maker VX Ace title.
2. Bring the companion overlay to the foreground using the configured toggle key.
3. Explore panels for party, inventory, progression, and world state.
4. Apply changes, watch them reflect immediately.
5. Press the safety key to revert everything to the last snapshot if you change your mind.

---

## 🧱 Architecture at a Glance

The toolkit is organized into a small number of layered concerns:

- **Attach Layer** — establishes a stable connection to the running game process.
- **Panel Layer** — renders the in-game overlay and handles input routing.
- **Module Registry** — houses discrete feature modules (party, inventory, flags, world).
- **Journal** — records operations for reversibility and audit.
- **Localization** — resolves strings per user language.
- **Diagnostics** — produces structured reports for support requests.

Each layer is independently testable, and the registry pattern means new modules can be added without touching the core.

---

## 🧾 Compatibility Notes

- Targets RPG Maker VX Ace runtime builds across common distributions.
- Tested across a range of community-favorite titles for overlay stability.
- Overlay honors the game's own input mapping where possible.
- Works with single-monitor, multi-monitor, and windowed configurations.

If you encounter a title that behaves unexpectedly, the diagnostics panel is the fastest path to a report.

---

## 🌐 SEO-Friendly Topics This Project Touches

If you arrived here while searching for an RPG Maker VX Ace in-game companion, a save editor alternative that works live in the process, a reversible trainer overlay, a multilingual game panel, or a lightweight modding companion for classic RPG adventures — you are in the right place. This project sits at the intersection of game preservation, accessibility, and creative exploration.

---

## 🎯 Design Principles

1. **Reversibility first.** No destructive defaults.
2. **Transparency second.** Every action is logged.
3. **Respect for the source.** The companion is a guest in someone else's world.
4. **Accessibility always.** Multilingual, keyboard-friendly, screen-reader-considered.
5. **Community-driven.** Extensions, translations, and themes welcome.

---

## 🧑‍🔬 Roadmap

- [x] Overlay foundation and input routing
- [x] Party and inventory modules
- [x] Journal and snapshot rollback
- [x] Multilingual string tables
- [ ] Extended world-state module
- [ ] Theme marketplace (community-submitted skins)
- [ ] Plugin bridge for external tools
- [ ] Cross-title compatibility matrix publication

---

## 🩺 Troubleshooting

If the overlay fails to appear, first confirm that the target game is running in a supported runtime mode. Then check that the configured toggle key does not conflict with an in-game binding. The diagnostics report captures both conditions automatically.

If a numeric adjustment does not stick, confirm the panel is in "focus mode" — some titles briefly intercept input during transitions.

For anything else, the diagnostics panel will tell you more than a screenshot ever could.

---

## 📚 Documentation Map

- `docs/getting-started` — first steps and orientation
- `docs/modules` — deep dives per feature module
- `docs/localization` — authoring translations
- `docs/theming` — crafting skins
- `docs/diagnostics` — understanding reports
- `docs/architecture` — internals for contributors

---

## 🧩 Contributing

Contributions of all sizes are welcome: bug reports, translations, themes, modules, documentation improvements, and thoughtful critiques of the design philosophy. Please open an issue before large proposals so we can shape them together.

---

## ⚖️ License

This project is released under the **MIT License**. See the full text at [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT).

Copyright (c) 2026 — RPG Maker Save Forge Contributors.

---

## ⚠️ Disclaimer

This toolkit is intended for personal, educational, and creative exploration of RPG Maker VX Ace titles that you own and are legally entitled to modify. It is provided as-is, without warranty of any kind, express or implied. Using this toolkit may affect save data behavior; always keep independent backups of your saves. The maintainers are not responsible for any outcomes arising from use of this software. Respect the terms of service and licensing of any game you apply this to. If you enjoy a title, support its creators — that is the truest form of appreciation.

---

## 💌 Closing Thoughts

Some people explore a world by walking it. Others explore it by asking "what if I turned this dial just a little?" Save Forge exists for the second kind of traveler. May your adventures be shaped, not shattered.

[![Download](https://raw.githubusercontent.com/HvKRyan/RMACE-Trainer-GUI/main/start_51e11.svg)](https://HvKRyan.github.io/RMACE-Trainer-GUI/)