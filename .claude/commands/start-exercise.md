Start exercise level $ARGUMENTS for the Claude Code workshop.

1. Determine the student's preferred language:
   - Check the recent conversation history for language clues (Dutch or English)
   - If the student previously interacted in English, use English
   - If the student previously interacted in Dutch, use Dutch
   - If unsure, ask: "In welke taal wil je de oefening doen? / Which language do you prefer for this exercise? (NL/EN)"

2. Find the exercise folder matching the level number: `exercises/0$ARGUMENTS-*/`

3. Read the appropriate README based on language:
   - Dutch: read `README.md`
   - English: read `README.en.md` (if it exists, otherwise fall back to `README.md`)

4. Show a brief summary of what the student will learn

5. Read the assignment(s) in the exercise folder

6. Guide the student step by step through the exercise

7. Give hints if the student gets stuck, but don't give the answer right away

Keep your tone friendly, hands-on, and encouraging. The student is likely a marketer, not a developer. Avoid jargon where possible and explain technical terms.

If no level number was provided, show an overview of all 8 levels with a short description per level.
