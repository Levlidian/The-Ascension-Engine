AI DUNGEON STORY STORAGE ENGINE
COMPLETE USER GUIDE (UPDATED)

==================================================
WHAT THIS ENGINE IS (PLAIN ENGLISH)
==================================================

This engine is a WORLD & CHARACTER STATE MANAGER.

It does NOT write prose for you.
It does NOT replace the AI.
It quietly manages consistency so the AI can write better.

It automatically tracks:
- Time, date, season, and holidays
- Cities, districts, and locations
- Travel (road trips, space travel, other dimensions)
- NPC emotions, trust, attraction, and romance
- Major and minor characters
- Clothing, mood, and behavior changes
- Escalation and consequences
- Response length and descriptive density

Think of it as a backstage crew:
You act. The AI performs. The engine keeps the world coherent.

==================================================
CRITICAL TRUTH (VERY IMPORTANT)
==================================================

The AI CANNOT read JavaScript.

The AI ONLY reads TEXT that is injected into context.

The script:
1. Watches what the player types
2. Updates hidden world state
3. Injects short, factual summaries into context
4. The AI reads those summaries as truth

This means:
YES — the script does the heavy lifting.
Story cards and memory stay minimal.

==================================================
WHAT HAPPENS EACH TURN (SIMPLIFIED)
==================================================

1. Player types an action
   Example: “I enter the bar.”

2. Input Modifier runs
   - Detects intent (movement, time, kindness, aggression, intimacy)
   - Updates world state

3. Context Modifier runs
   - Injects:
     • Time & date
     • Location & district
     • Characters & emotions
     • Travel mode & environment
     • Response style
     • Escalation

4. AI reads the injected text
5. AI writes the scene respecting those facts

The AI NEVER sees the code.

==================================================
WHY NOTHING APPEARS ON TURN ONE
==================================================

On an empty scenario:
- No player input exists yet
- Scripts have nothing to react to
- The AI sees a blank page

THIS IS NORMAL.

Always seed ONE of the following:
- A short opening paragraph in Story
- A brief Memory entry

Example Story seed:
“Rain slicks the streets. Neon hums. A bar waits beneath the lights.”

==================================================
WHAT YOU EDIT (NO CODING REQUIRED)
==================================================

You NEVER need to edit logic.

You ONLY edit:
- The EDITABLE DATA BLOCK in the Library
- Story text
- Memory
- Minimal Story Cards

--------------------------------------------------
EDITABLE DATA BLOCK (SAFE)
--------------------------------------------------

You can safely edit:
- Characters (add unlimited major & minor NPCs)
- Races/species
- Clothing options
- Personality traits
- Holidays & festivals
- Cities, districts, locations
- Name pools for random NPCs
- Dialogue flavor pools
- Response length preference

DO NOT edit anything marked:
“LOGIC BELOW – DO NOT EDIT”

==================================================
CHARACTERS (MAJOR & MINOR)
==================================================

Each character supports:
- Personality traits
- Physical description
- Clothing (changes by mood/situation)
- Mannerisms
- Emotional state
- Trust & attraction
- Romance stage
- Race/species

Minor NPCs are generated automatically from pools:
- First & last names
- Races
- Traits
- Clothing styles
- Mannerisms
- Dialogue flavor

This gives the AI a large variety of voices and behaviors.

==================================================
CLOTHING & MOOD
==================================================

Clothing automatically shifts based on:
- Mood
- Situation
- Public vs private spaces
- Intimacy or tension

You do not need to track outfits manually.

==================================================
TIME & CALENDAR SYSTEM
==================================================

Automatic:
- Every 5 player turns → 10 minutes pass
- Time rolls into hours, days, seasons, years

Player-controlled acceleration:
- “wait”
- “rest”
- “sleep”
- “skip ahead”

Time checking (genre-agnostic):
- Modern: “check your phone”
- Fantasy: “check the sun”
- Sci-fi: “check your HUD”

When the player checks time, the engine FORCES the AI
to include the current time in its response.

==================================================
HOLIDAYS & FESTIVALS
==================================================

Named events live in the holidays block.

The AI will naturally:
- Reference celebrations
- Adjust mood
- Change crowd behavior
- Alter atmosphere

You only need to name them and describe them once.

==================================================
TRAVEL & ENVIRONMENTS
==================================================

Supported:
- Stationary (city play)
- Road trips
- Wilderness travel
- Space travel
- Other dimensions / realities

The engine tracks:
- Travel mode
- Environment type

The AI adjusts descriptions automatically.

==================================================
RESPONSE STYLE CONTROL
==================================================

Players can naturally influence verbosity:

Examples:
- “describe more”
- “slow down”
- “be detailed”
- “summarize”
- “skip ahead”

This changes RESPONSE STYLE:
- Short
- Normal
- Rich
- Novel

This prevents repetitive AI phrasing and encourages variety.

==================================================
STORY CARDS (KEEP THEM MINIMAL)
==================================================

Story cards are REFERENCE ONLY.

Recommended:
- Character card: name, core personality, race
- Location card: name, vibe
- World card: 1–2 rules of reality

DO NOT dump lore.
DO NOT write long essays.

The engine handles continuity.

==================================================
INNERSELF INTEGRATION (VERY IMPORTANT)
==================================================

InnerSelf is OPTIONAL.

What InnerSelf does:
- NPC inner thoughts
- Goals, secrets, planning

What THIS engine does:
- World state
- Time
- Locations
- Emotions
- Romance
- Context clarity

THEY WORK TOGETHER.

--------------------------------------------------
CRITICAL INNERSELF SETUP STEPS
--------------------------------------------------

When adding InnerSelf to this engine:

1. Paste InnerSelf code into the Library tab
2. In the Input Modifier:
   DELETE Story Engines top:
   const modifier = (text) => { ... }

3. In the Context Modifier:
   DELETE Story Engines top:
   const modifier = (text, stop) => { ... }

4. KEEP the calls already present in this engine:
   - InnerSelfInput(text)
   - InnerSelfContext(text, stop)

5. DO NOT replace the Output Modifier.
   The Output Modifier included in this engine
   IS REQUIRED for InnerSelf compatibility.

Paste the Story Storage Engine as guided by Lewdlead, delete the script below where she says to add other mods here.

==================================================
COMMON MISTAKES TO AVOID
==================================================

- Overwriting logic sections
- Duplicating modifier wrappers
- Overloading story cards
- Expecting scripts to write prose
- Repeating lore every turn

==================================================
FINAL MENTAL MODEL
==================================================

You play naturally.
The engine remembers.
The AI writes better because it knows more.

If the world feels alive and consistent,
the engine is doing its job.

==================================================
END OF GUIDE
==================================================
