
CHOOSE A MONSTER – MONSTER ASCENSION ENGINE v3.0
COMPLETE PLAYER & EDITOR README (AI DUNGEON – TXT)

================================================
WHAT THIS ENGINE IS
================================================

This engine allows you to play as a monster, not a hero.

You begin unformed and evolve through:
- Rank and Level progression
- Origin, Adaptive, and Scar mutations
- Humanoid Drift and Decay
- Nemesis escalation
- Size growth
- Optional ascension paths

Everything reacts to what you write.
There are no menus, stats, or buttons.

================================================
INSTALLATION
================================================

1. Create a new Custom Adventure in AI Dungeon
2. Paste the FULL engine into Scripts → Input Modifier
3. Save and begin play

INNER SELF NOTE:
If using InnerSelf, delete the top `const modifier` declaration
before inserting InnerSelf into the engine.

================================================
MODULE TOGGLES
================================================

The following can be safely enabled or disabled:

ORIGIN_EVOLUTION
ADAPTIVE_EVOLUTION
SCAR_SYSTEM
HUMANOID_DRIFT
HUMANOID_DECAY
NEMESIS_SYSTEM
SIZE_SYSTEM
EVOLUTION_LINES
DEMON_LORD_SYSTEM
TITAN_SYSTEM
STORY_CARDS

================================================
MANDATORY START COMMAND
================================================

You MUST declare an origin before play begins.

COMMAND:
[Origin: Wolf]

Accepted Origins include:
Wolf, Black Hound, Ghoul, Barrow Revenant, Stone Golem,
Stonebound Warden, Ent, Wraith, Serpent, Large Spider,
Chimera, Skin-Stealer, Fey Abomination, Drake, Ash Drake,
Demon, Night Warden, Bog Horror, Plague Host, Deep Wyrm

================================================
XP & PROGRESSION (AUTOMATIC)
================================================

XP is gained every turn.

Violent actions (kill, fight, hunt, attack) give more XP.
Non-violent actions still progress evolution.

No command needed.

================================================
SCAR TRIGGERS
================================================

Scar mutations may trigger if your input includes:

wounded
burned
maimed
broken
scarred

Scars are permanent.

================================================
HUMANOID DRIFT TRIGGERS
================================================

Drift may increase if your input includes:

talk
speak
negotiate
bargain
reason
protect
guard
spare
hesitate
refuse
listen

Drift may DECREASE if your input includes:

slaughter
massacre
devour
rend
rip apart
maul
feast
consume

================================================
UNLOCKED HUMANOID CAPABILITIES
================================================

2 Drift: You can speak clearly
4 Drift: You can disguise yourself
6 Drift: Others may follow you

================================================
ASCENSION COMMANDS (SS RANK)
================================================

When prompted at SS Rank:

COMMAND:
demon lord

RESULT:
Ascend through dominion and authority

OR

COMMAND:
titan

RESULT:
Ascend through mass and world-altering scale

OR

TYPE NOTHING AND CONTINUE PLAY
to refuse ascension and remain a monster

This choice is permanent.

================================================
NEMESIS SYSTEM COMMANDS
================================================

AUTOMATIC NEMESIS CREATION:
Triggered if your input includes:

escaped
retreated
survived

These create damaged hunters automatically.

------------------------------------------------
MANUAL NEMESIS CREATION (PLAYER-COMMANDED)
------------------------------------------------

BOTH lines must appear in the SAME TURN:

Nemesis Name: Valcerin
Nemesis Personality: Methodical

VALID PERSONALITY KEYS:
relentless
methodical
vengeful
zealous
pragmatic

================================================
NEMESIS REMOVAL
================================================

If your input includes:

killed
slain
destroyed

The oldest active nemesis is removed.

================================================
TIME & WORLD PRESSURE
================================================

Time advances automatically every few turns.
Day shifts to Night.
Seasons change every 30 days.

Night increases danger and aggression.

================================================
STORY CARDS (AUTO)
================================================

The engine maintains:

Self Appraisal
Nemesis Escalation

These cards auto-update and should NOT be edited manually.

================================================
WRITING GUIDELINES
================================================

DO:
- Describe intent, scale, damage, and consequence
- Let the world react

DO NOT:
- Force mechanics
- Declare mutations manually
- Use stat language

================================================
FINAL NOTE
================================================

You are not grinding power.
You are becoming a problem.

The world will respond.
