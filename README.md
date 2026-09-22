![preview](https://raw.githubusercontent.com/priteshsah2024-dotcom/Oxomo-Luau-Style-Guide/main/promo_e5fd9e.svg)
# 🧭 Oxomo Conventions Companion

A living, breathing style compass for Roblox/Luau teams who refuse to let their codebase drift into chaos.

[![Download](https://raw.githubusercontent.com/priteshsah2024-dotcom/Oxomo-Luau-Style-Guide/main/latest_62c8ede.svg)](https://priteshsah2024-dotcom.github.io/Oxomo-Luau-Style-Guide/)

![Luau](https://img.shields.io/badge/Language-Luau-00A2FF?style=for-the-badge&logo=lua&logoColor=white)
![Roblox](https://img.shields.io/badge/Platform-Roblox-E2231A?style=for-the-badge&logo=roblox&logoColor=white)
![MIT](https://img.shields.io/badge/License-MIT-3DA639?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Status](https://img.shields.io/badge/Status-Actively%20Maintained-6E4AFF?style=for-the-badge)
![Year](https://img.shields.io/badge/Release-2026-FF6B35?style=for-the-badge)

---

## 🌌 Why This Repository Exists

Every studio eventually hits the same wall: one developer writes `local player = game.Players.LocalPlayer`, another writes `local plr = Players.LocalPlayer`, and a third names it `theGuyWhoClicked`. Six months later, nobody remembers what `tbl2` was supposed to represent, and onboarding a new scripter feels like handing them a treasure map drawn in the dark.

**Oxomo Conventions Companion** is the answer to that slow-motion confusion. It is not merely a ruleset — it is an entire philosophy bundled into tooling, examples, and a shared vocabulary. Think of it as a lighthouse: it does not sail the ship for you, but it makes sure you never crash into the rocks of inconsistency.

This project grew out of the original *Oxomo-Coding-Conventions* reference, expanded into a full companion ecosystem for teams who want their Luau to read like prose rather than static.

---

## 🎯 Core Mission

We believe code is a form of writing, and writing deserves an editor. This repository provides:

- A canonical conventions document tailored to Roblox/Luau realities
- Lint-friendly examples that can be dropped into any Studio workflow
- A review checklist that works for solo devs and 40-person teams alike
- Reference snippets for common patterns: services, signals, OOP, state, and networking
- Guidance on naming, scoping, error handling, and module architecture

Everything here is designed to be **adoptable in pieces**. You do not need to swallow the whole whale — start with naming, then graduate to structure.

---

## 🧩 Feature List

- 🎨 **Style Spectrum** — conventions that scale from tiny game jams to long-running live-service projects
- 🔍 **Audit-Ready Examples** — before/after snippets showing exactly what to change and why
- 🧠 **Rule Rationale** — every convention comes with a short "why," because blind rules get ignored
- 📚 **Multilingual Documentation Support** — translated summaries for global teams, with the ability to add more
- 🖥️ **Responsive Documentation UI** — the companion site renders cleanly on desktop, tablet, and mobile
- 🛎️ **Assisted Guidance Around the Clock** — community maintainers respond to questions in every timezone
- 🧪 **Testable Patterns** — Luau examples structured to work with common test harnesses
- 🔁 **Versioned Convention Releases** — pin your project to a convention snapshot and upgrade on your schedule
- 🧭 **Onboarding Flow** — a curated path for new contributors, interns, and returning veterans
- 🌐 **SEO-Friendly Structure** — headings, anchors, and cross-links crafted so search engines find each rule quickly

---

## 🏗️ Repository Layout

A bird's-eye view of how the pieces fit together:

- `docs/` — the long-form conventions, split by theme
  - `naming/` — identifiers, casing, prefixes, and the eternal `is`/`has` debate
  - `structure/` — module layout, service boundaries, folder discipline
  - `style/` — formatting, comments, whitespace, and line-length preferences
  - `patterns/` — OOP idioms, state management, event-driven design
  - `networking/` — RemoteEvent and RemoteFunction hygiene
- `examples/` — runnable Luau samples, each one a miniature case study
- `checklists/` — printable review sheets for pre-merge validation
- `translations/` — localized summaries of the core conventions
- `tools/` — helper scripts that scan a codebase for convention drift
- `roadmap/` — what is coming in future convention releases

---

## 🚀 Getting Started Without the Usual Friction

You do not need to memorize anything. Begin with the checklist that matches your current pain:

1. Open `checklists/pre-merge.md` and skim it once.
2. Pick **three rules** that resonate with your team.
3. Apply them to a single module — ideally a small one.
4. Run the convention scanner in `tools/` to see the delta between your code and the recommended patterns.
5. Repeat weekly. Consistency compounds; it does not arrive in a single afternoon.

If you prefer a guided path, read `docs/onboarding.md` first. It is written for humans, not compilers.

---

## 🧬 A Taste of the Conventions

Conventions are only useful when they are memorable. Here is a small sample of the rules included:

- Prefer descriptive names over abbreviations — `PlayerService` beats `PSvc`
- Every module begins with a short comment describing its responsibility in one sentence
- Never expose internal state directly; expose behavior instead
- Use `assert` and structured error tables for recoverable failures
- Keep functions under 40 lines where practical; if longer, extract a helper
- Group related services at the top of the file to make dependencies obvious
- Prefer composition over inheritance unless the model truly is a subtype

Each of these is expanded in the `docs/` directory with counterexamples and edge cases.

---

## 🎨 Responsive Documentation UI

The companion documentation site is designed with a responsive layout that adapts fluidly from ultrawide monitors to phones. Sidebar navigation collapses gracefully, code blocks reflow without horizontal scrolling where possible, and dark/light themes are both first-class citizens. The goal is simple: reading conventions should feel effortless, whether you are at a desk or on a bus.

---

## 🌍 Multilingual Support

Conventions cross borders. To help distributed teams stay aligned, the repository ships with translated summaries of the core rules. Currently supported summary languages expand over time, and contributions for additional languages are welcomed. The English long-form remains the reference for edge-case wording, but the summaries are written to be genuinely useful, not word-for-word mirrors.

---

## 🛎️ Around-the-Clock Assistance

Questions do not respect business hours, so neither does the maintainer group. Support channels are monitored continuously across timezones, and new issues are triaged with the same care whether they arrive at noon or at 3 AM. For urgent coordination, refer to the pinned discussion thread where maintainers and contributors coordinate in real time.

---

## 🧪 Testing and Validation

Each example under `examples/` ships with a small validation script that confirms the pattern behaves as documented. This keeps the repository honest: if a convention changes, the examples change with it, and the validation confirms nothing silently broke.

---

## 🤝 Contributing

Contributions are welcome and encouraged, provided they respect a few ground rules:

- Every new rule must include a short rationale
- Examples must be runnable and minimal
- Translations must be reviewed by at least one native speaker
- Pull requests should link to the checklist item they address
- Discussion is preferred over silent rewrites of existing conventions

See `docs/contributing.md` for the full guide. First-time contributors are especially welcome, and there is a dedicated label for issues that are ideal starting points.

---

## 🗺️ Roadmap Highlights for 2026

- A convention linter integration for popular editors
- Expanded examples covering DataStore patterns and replication edge cases
- Additional translated summaries for wider team coverage
- A migration guide for teams moving from ad-hoc styles to Oxomo conventions
- Interactive web playground for testing snippets against the recommended style

The roadmap is maintained in the `roadmap/` directory and evolves with community feedback.

---

## ⚠️ Disclaimer

This repository provides coding conventions, documentation, and example code intended for educational and team-alignment purposes. It does not guarantee performance, security outcomes, or compatibility with every project configuration. Users are responsible for adapting the conventions to their own codebase, reviewing all changes before applying them in a live environment, and complying with the terms of the platforms they build upon. The maintainers are not liable for any direct or indirect consequences arising from the use of the materials provided. Always back up your work and test thoroughly.

---

## 📜 License

This project is released under the MIT License. See the full text at:

https://opensource.org/licenses/MIT

Copyright (c) 2026 Oxomo Conventions Companion contributors.

---

## 💬 Final Thought

Style guides are not chains — they are guardrails on a mountain road. They do not stop you from driving; they make sure the drive is worth remembering. Welcome aboard, and may your Luau always compile on the first try.

[![Download](https://raw.githubusercontent.com/priteshsah2024-dotcom/Oxomo-Luau-Style-Guide/main/latest_62c8ede.svg)](https://priteshsah2024-dotcom.github.io/Oxomo-Luau-Style-Guide/)