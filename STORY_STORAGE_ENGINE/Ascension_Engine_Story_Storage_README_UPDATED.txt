THE ASCENSION ENGINE SERIES
STORY STORAGE ENGINE
UPDATED README (FINAL)

==================================================
WHAT THIS ENGINE IS
==================================================

The Story Storage Engine is a long-form narrative support system for AI Dungeon.

It does NOT write the story for you.
It does NOT replace the AI.
It exists to quietly remember the world so the AI can stay consistent.

Think of it as the world’s memory, social awareness, and sense of time.

The AI still writes prose.
You still play naturally.
The engine handles continuity.

==================================================
WHAT PROBLEM THIS SOLVES
==================================================

Without an engine:
- NPCs forget past behavior
- Time feels meaningless
- Locations blur together
- Relationships reset
- Long stories collapse under their own weight

With this engine:
- The world remembers
- People react socially
- Time passes naturally
- Rumors spread
- Quiet days exist
- Years actually matter

==================================================
HOW IT WORKS (NON-TECHNICAL)
==================================================

The AI cannot read scripts.

Instead, the engine:
1. Watches what the player types
2. Updates hidden world state
3. Injects short, factual summaries into context
4. The AI reads those summaries as truth

Nothing magical.
No mind reading.
Just structured reminders.

==================================================
WHY IT MAY FEEL “SMALLER”
==================================================

Nothing was removed.

Earlier versions repeated the same ideas in multiple places.
The final version merges overlapping systems.

This makes the script:
- Shorter to read
- Easier to maintain
- Stronger per line

Functionality was preserved.
Redundancy was removed.

==================================================
TIME & YEARS
==================================================

Time is tracked at multiple scales:
- Minutes, hours, days
- Months and seasons
- Years

Defaults:
- Every 5 player actions = 10 minutes
- “wait”, “rest”, “sleep” accelerate time
- Time checks force the AI to state the time

This engine is designed for stories that span YEARS.

==================================================
SLICE-OF-LIFE SYSTEMS
==================================================

The engine supports everyday life without simulation.

It includes:
- Ambient life at locations
- Seasonal atmosphere
- Weekday vs weekend behavior
- Neighborhood-specific vibes
- Routine disruption cues
- Quiet “nothing happens” moments

These are suggestions, not rules.
The AI chooses how to express them.

==================================================
CHARACTERS & NPCs
==================================================

Supports unlimited:
- Major characters
- Minor characters
- One-off NPCs

Each can have:
- Personality traits
- Emotional state
- Mannerisms
- Clothing logic
- Race/species
- Jobs and usual hangouts

Minor NPCs can be generated automatically from editable pools.

==================================================
RELATIONSHIPS
==================================================

The engine tracks:
- Friendship
- Romance
- Hostility
- Trust and attraction

Behavior changes naturally:
- Physical distance
- Tone of voice
- Habits and mannerisms

No meters required.
No UI required.

==================================================
FRIEND GROUPS & PACKS
==================================================

Groups are treated as social entities.

They can be:
- Loyal
- Strained
- Fractured

This affects:
- Who speaks
- Who protects whom
- Who gets excluded
- How tension appears in scenes

Group type is reference-agnostic:
friends, packs, crews, families, circles.

==================================================
REPUTATION & STORIES
==================================================

Reputation is social, not numeric.

NPCs:
- Talk about you
- Misremember events
- Exaggerate behavior
- Form opinions second-hand

Stories about you evolve over time:
- Fresh
- Distorted
- Mythic
- Forgotten

This applies even when you are not present.

==================================================
MEMORY, FORGETTING & NOSTALGIA
==================================================

The world remembers imperfectly.

Over years:
- Details fade
- Emotional truth remains
- Stories soften or harden
- Some events vanish entirely

This keeps long stories believable.

==================================================
HOME BASE EFFECTS
==================================================

Certain places act as emotional anchors.

Returning:
- Lowers tension
- Restores familiarity

Leaving:
- Creates subtle dissonance

Changing:
- Creates nostalgia or loss

“Home” is narrative, not mechanical.

==================================================
PLAYER CONTROL
==================================================

Players can influence:
- Pacing
- Detail level
- Time progression

Naturally, through language:
- “describe more”
- “summarize”
- “skip ahead”
- “wait”

No commands required.

==================================================
STORY CARDS (KEEP THEM MINIMAL)
==================================================

Story cards are references, not lore dumps.

Recommended:
- Character name + core traits
- Location name + vibe
- World rule or genre note

The engine handles continuity.

==================================================
INNERSELF COMPATIBILITY (IMPORTANT)
==================================================

InnerSelf is optional.

If using InnerSelf:
1. Paste InnerSelf into the Library
2. DELETE InnerSelf’s own modifier wrappers
   in Input and Context
3. Keep the calls already in this engine:
   - InnerSelfInput
   - InnerSelfContext
4. DO NOT replace the Output Modifier

Failure to do this will cause errors.

==================================================
WHAT NOT TO EDIT
==================================================

Do NOT edit:
- Logic sections
- Functions marked “DO NOT EDIT”
- Modifier wrappers

You only edit:
- Editable data blocks
- Text lists
- Descriptions

==================================================
FINAL MENTAL MODEL
==================================================

You play.
The engine remembers.
The AI writes better because it knows more.

The world does not pause when you stop looking.
It ages, gossips, forgets, and adapts.

That is the engine’s purpose.

==================================================
END OF README
==================================================
