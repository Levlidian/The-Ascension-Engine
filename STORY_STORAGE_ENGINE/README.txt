STORY STORAGE ENGINE
README.txt
Beginner-Friendly Guide (No Coding Required)

WHAT THIS IS
This system is a story memory and awareness engine.
It stores world facts, characters, locations, tone, and time.
It quietly guides the AI every turn.

WHAT IT DOES
- Remembers who exists
- Remembers where you are
- Tracks time, date, and season
- Maintains mood and atmosphere
- Controls how characters sound when they speak
- Keeps scenes consistent across turns

WHAT IT DOES NOT DO
- No combat rules
- No stat rolling
- No forced outcomes
- No player restriction

FILES (DO NOT RENAME)
LIBRARY_STORY_STORAGE_ENGINE
Main story data. You edit this file.

CONTEXT_STORY_STORAGE_ENGINE
Injects story facts into every AI response.

INPUT_STORY_STORAGE_ENGINE
Tracks turns, time, and player intent.

OUTPUT_INNERSELF_SAFE_STORY_STORAGE_ENGINE
Final output safety pass.

INNERSELF SETUP (CRITICAL)
Only the InnerSelf LIBRARY is required.
Place the InnerSelf library ABOVE the Library Story Storage Engine.
Do not include InnerSelf logic or behaviors.

SAFE TO EDIT
- Names
- Descriptions
- Mood words
- Lists
- Characters
- Locations
- Groups
- World rules (text only)

DO NOT EDIT
- Function names
- Brackets { }
- Commas
- Code logic

TIME SYSTEM (AUTOMATIC)
Every 5 turns: +10 minutes
WAIT: +30 minutes
SLEEP: +8 hours

Recognized commands:
check time
what day is it
what season is it
is there an event today
wait
sleep

FINAL NOTE
Treat this engine like a living story encyclopedia.
