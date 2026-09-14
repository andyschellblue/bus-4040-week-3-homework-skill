markdown
---
name: memo-formatter
description: Formats rough notes or bullet points into a professional business memo with a standard header block, purpose, background, recommendation, and next steps.
---

# Business Memo Formatter

## What this skill does
Takes unstructured notes, bullet points, or a stream-of-consciousness summary and turns them into a clean, professional business memo following a standard format.

## When to use this skill
Use this skill whenever the user asks to:
- "Turn these notes into a memo"
- "Write this up as a memo"
- "Format this as a business memo"
- "Draft a memo about [topic]"

## Output format

Every memo should follow this structure:

MEMORANDUM

TO:      [Recipient(s)]
FROM:    [Sender]
DATE:    [Date]
RE:      [Subject line — short and specific]

PURPOSE
[1–2 sentences stating why this memo exists and what decision or action it supports.]

BACKGROUND
[Relevant context the reader needs. Keep it factual and concise.]

RECOMMENDATION
[The specific recommendation or conclusion, stated clearly and directly.]

NEXT STEPS
[A short bulleted list of concrete action items, ideally 
## Instructions

1. If the user's notes don't specify a TO, FROM, or DATE, ask them or use reasonable placeholders like `[Recipient Name]`.
2. Keep the tone professional and concise — this is a business document, not an email or casual message.
3. Do not invent facts, numbers, or decisions that weren't in the user's original notes. If something is unclear, flag it rather than guessing.
4. Bullet points in the Next Steps section should be action-oriented (start with a verb) and specific.
5. Keep the whole memo under one page's worth of content unless the user's source material genuinely requires more.

## Example

**Input notes:**
"need to tell the team we're switching project management tools from Trello to Asana starting next month, IT is handling migration, everyone needs to finish current Trello boards by end of this month, training session scheduled for the 15th"

**Output:**

MEMORANDUM

TO:      Project Team
FROM:    [Sender Name]
DATE:    [Date]
RE:      Transition from Trello to Asana

PURPOSE
This memo announces the team's transition from Trello to Asana for project management, effective next month.

BACKGROUND
The team currently manages projects in Trello. Starting next month, all project management will move to Asana. IT will handle the technical migration.

RECOMMENDATION
All team members should complete and close out current Trello boards by the end of this month to ensure a clean transition.

NEXT STEPS
- Finish and archive all active Trello boards by end of month
- Attend the Asana training session on the 15th
- Direct migration questions to IT