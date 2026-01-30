# MONARCH ASCENSION ENGINE v1.2

![Version](https://img.shields.io/badge/version-1.2-blue)
![AI Dungeon](https://img.shields.io/badge/AI%20Dungeon-Compatible-success)
![Monster Engine](https://img.shields.io/badge/Monster--Engine-Ready-purple)
![Solo Leveling](https://img.shields.io/badge/Inspiration-Solo%20Leveling-black)
![License](https://img.shields.io/badge/license-Free%20Use-lightgrey)

**Solo Leveling–Inspired • Monster-Engine Appraisal System**  
_AI Dungeon – Ready to Paste_

---

## 📌 Table of Contents

- [Overview](#overview)
- [Core Features](#core-features)
- [Player Guide](#player-guide)
  - [Progression](#progression)
  - [Ability Evolution](#ability-evolution)
  - [Ability Categories](#ability-categories)
  - [Monarch Paths](#monarch-paths)
  - [Army System](#army-system)
  - [Self Appraisal](#self-appraisal)
- [Modder Guide](#modder-guide)
  - [Design Philosophy](#design-philosophy)
  - [Adding Abilities](#adding-abilities)
  - [Progression Tuning](#progression-tuning)
  - [Compatibility](#compatibility)
- [Intended Experience](#intended-experience)
- [License](#license)

---

## Overview

The **Monarch Ascension Engine** is a narrative-driven progression framework inspired by *Solo Leveling*. It converts freeform storytelling into a structured power climb where **combat, magic, and command authority evolve organically through use**.

There are no menus.  
No point-buy screens.  
Only actions, consequences, and growth.

A single, persistent **Self Appraisal** story card tracks your ascent automatically using Monster-Engine–style logic.

---

## Core Features

- 📈 Dynamic leveling and rank progression  
- 🧬 Ability evolution through narrative use  
- 👑 Six unique Monarch paths  
- ⚔️ Army command system (Knights, Elites, Commanders)  
- 📜 Auto-updating Monster-Engine self appraisal  
- 🧠 Deterministic, AI-safe keyword logic  

---

## Player Guide

### Progression

- You begin at **Level 1, Rank E** with dormant Monarch authority.
- XP is awarded automatically based on narration:
  - **High-intensity actions** (fight, kill, survive, dominate) grant more XP.
  - **Low-intensity actions** (train, explore, study, recover) grant less XP.
- Level requirement: `Level × 20 XP`.
- Rank updates automatically as levels increase.

You never issue system commands to level up.  
Your narration *is* the trigger.

---

### Ability Evolution

Abilities grow through **repeated narrative use**.

- Each ability has **4 tiers**.
- Each tier requires `(current tier + 1) × 3` successful narrative triggers.
- When an evolution occurs, the system announces it automatically.

You do not select upgrades.  
Your behavior defines them.

---

### Ability Categories

#### Authority Abilities (30)
Physical and instinctive growth such as strength, speed, perception, killing intent, survival, and dominance.

#### Magic Abilities (20)
Elemental and conceptual magic paths including shadow, frost, fire, lightning, gravity, time, space, soul, and void.

#### Monarch Abilities
Exclusive powers unlocked after **Rank A**.  
Each Monarch possesses **5 unique abilities**, each evolving through 4 tiers.

---

### Monarch Paths

- **Shadow** – Darkness, silence, undead dominion  
- **Beast** – Predation, evolution, instinct  
- **Frost** – Absolute cold and frozen time  
- **Decay** – Entropy, rot, extinction  
- **Iron** – Defense, siege, unbreakable form  
- **Destruction** – Cataclysm and annihilation  

Before awakening, only a **hint title** is displayed to preserve narrative mystery.

---

### Army System

Unlocked automatically upon reaching **Rank A**.

Narrative commands:
```text
arise
arise 5
arise elite
arise commander 2
```

Limits:
- Total Army Size: **200**
- Elites: **10**
- Commanders: **5**

Elites and Commanders are generated with unique names and personalities.

---

### Self Appraisal

A permanent story card titled **Self Appraisal** displays:

- Rank, Level, and XP  
- All unlocked abilities and tiers  
- Army composition  
- Monarch authority state  

The card updates every turn and is fully Monster-Engine compliant.

---

## Modder Guide

### Design Philosophy

- Deterministic keyword-based triggers  
- No UI or menu dependencies  
- No RNG-based power spikes  
- Campaign-safe, persistent logic  

This engine is designed to be **extended**, not rewritten.

---

### Adding Abilities

Add new abilities to:
- `AUTHORITY_ABILITIES`
- `MAGIC_ABILITIES`
- `MONARCH_ABILITIES[monarchId]`

Rules:
- Exactly **4 tiers** per ability
- The **first word** of the base ability name is used as the keyword trigger

Example:
```js
"Blood Control": [
  "Blood Control",
  "Hemokinesis",
  "Crimson Dominion",
  "Absolute Blood Rule"
]
```

---

### Progression Tuning

- XP values: `gainXP()`
- Tier requirements: `evolveAbility()`
- Level curve: `level * 20`
- Army limits: `processArise()`

All progression logic is centralized and easy to modify.

---

### Compatibility

- InnerSelf compatible (optional)
- Uses only `state` and `storyCards`
- Safe for long-running AI Dungeon campaigns
- Fully Monster-Engine compliant

---

## Intended Experience

This engine supports:

- Power-fantasy escalation  
- Long-form solo campaigns  
- Monarch, dungeon-core, or evolution narratives  
- Story-driven progression where **actions define power**  

You are not choosing a build.

You are becoming one.

---

## License

Free to use, modify, fork, and expand for personal or public AI Dungeon scenarios.
