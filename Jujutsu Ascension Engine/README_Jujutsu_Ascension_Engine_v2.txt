
JUJUTSU ASCENSION ENGINE v2
README — COMPLETE GUIDE (BEGINNER FRIENDLY)

====================================================
WHAT THIS ENGINE IS
====================================================

The Jujutsu Ascension Engine v2 is a narrative-driven progression and combat system
inspired by Jujutsu Kaisen. It is designed for AI Dungeon-style storytelling,
where the AI reacts dynamically to player actions.

This is NOT a video game engine.
It is a ruleset that lives inside the story itself.

The engine tracks:
- Your sorcerer’s growth
- Cursed energy condition
- Techniques and domains
- Near-death awakenings
- Black Flash events
- World and NPC reactions

All of this happens automatically while you write normally.

====================================================
WHAT THIS ENGINE DOES AUTOMATICALLY
====================================================

You DO NOT need to type commands like a game.

The engine:
- Reads what you write
- Detects combat, danger, healing, and domain usage
- Adjusts your stats invisibly
- Updates a Story Card called “Sorcerer Appraisal”

You simply play the story.

====================================================
CORE DATA STORED BY THE ENGINE
====================================================

The engine stores one main object:

state.sorcerer

Inside it are:

- level (1–100)
- grade (Grade 4 → Special Grade)
- xp (experience)
- cursedEnergy state
- innate technique
- unlocked abilities
- domain status
- black flash count
- bloodline traits
- defensive techniques
- near-death flag
- entity type (Human / Simurian / Cursed Spirit)

You never need to edit these manually.

====================================================
CURSED ENERGY STATES
====================================================

Your cursed energy degrades naturally:

Overflowing
Abundant
Steady
Strained
Flickering
Depleted
Burned Out

Low energy prevents techniques.
Burned Out means no techniques at all.

====================================================
BLACK FLASH
====================================================

Black Flash:
- Cannot be chosen by the player
- Triggers only during combat narration
- Has ~1% chance (higher in Flow State)
- Instantly restores cursed energy
- Grants massive XP
- Can unlock Domains early

If it happens, the engine announces it.

====================================================
DOMAINS & DEFENSE
====================================================

Domain Expansion:
- Unlocks at Grade 1 OR after 5 Black Flashes
- Automatically detected from narration

Simple Domain:
- Unlocks at Grade 2
- Neutralizes sure-hit effects only

Falling Blossom Emotion:
- Unlocks at Grade 2
- Dodges attacks via continuous motion

====================================================
HEAVENLY RESTRICTION
====================================================

10% chance at character creation.

If you have it:
- No cursed energy
- No techniques
- No domain
- Extreme physical stats
- Physical power scales by grade

You play like Toji or Maki.

====================================================
ENTITY TYPES
====================================================

The engine detects special identities via narration:

- Simurian
- Cursed Spirit

These affect:
- NPC reactions
- Curse behavior
- World pressure

====================================================
FOR PLAYERS: HOW TO PLAY
====================================================

1. Write naturally.
2. Describe actions, emotions, and combat.
3. Never ask for stats.
4. Check the “Sorcerer Appraisal” Story Card to see growth.
5. Let failure happen. Power comes from survival.

That’s it.

====================================================
FOR CREATORS: ADDING A NEW CURSED TECHNIQUE
====================================================

You do NOT need coding experience.

Follow these steps carefully.

------------------------------------
STEP 1: FIND THIS SECTION
------------------------------------

INNATE_TECHNIQUES = [

This is a list of techniques.

------------------------------------
STEP 2: COPY AN EXISTING TECHNIQUE
------------------------------------

Copy everything from:

{
  name: "...",
  domain: {...},
  abilities: [...]
}

------------------------------------
STEP 3: CHANGE THE WORDS ONLY
------------------------------------

DO NOT change symbols like:
{ } [ ] : ,

ONLY change text inside quotes.

Example:

name: "Your Technique Name"

------------------------------------
STEP 4: ABILITIES RULES
------------------------------------

You must have EXACTLY three abilities:

1. Base
2. Reversal
3. Maximum

Format:

{ type:"Base", n:"Name", d:"Description" }

------------------------------------
STEP 5: DOMAIN RULES
------------------------------------

A domain must include:

- name
- description
- sureHit

------------------------------------
STEP 6: SAVE AND TEST
------------------------------------

Paste engine into AI Dungeon.
Start a new story.
Check if a technique appears.

If the story crashes:
- You changed punctuation
- Or removed a comma

Undo and try again.

====================================================
SAFE EDITING RULES (VERY IMPORTANT)
====================================================

✔ You may:
- Add techniques
- Change descriptions
- Add new curse archetypes

✘ You must NEVER:
- Rename functions
- Delete “if (typeof …)” lines
- Rename modifier
- Add duplicate variable names

====================================================
WHY THIS ENGINE IS SAFE
====================================================

- Redeclaration-safe
- Paste-safe
- No overwrites
- No infinite loops
- No player exploitation

====================================================
FINAL NOTE
====================================================

This engine is designed to feel unfair, dangerous, and earned.

You are not special.
You become special.

Survive long enough.

====================================================
END OF README
====================================================
