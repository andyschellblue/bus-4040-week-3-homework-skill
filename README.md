# bus-4040-week-3-homework-skill

## What This Skill Does

This repository contains a Claude Skill called **memo-formatter**. It takes rough, unstructured notes — bullet points, a stream-of-consciousness paragraph, or a quick voice-to-text dump — and turns them into a clean, professional business memo with a standard format: a header block (TO/FROM/DATE/RE), a Purpose section, Background, a Recommendation, and a bulleted Next Steps list.

## How the Skill Works

The skill lives in `memo-formatter/SKILL.md`. It's a markdown file with:
- A short description of what the skill does and when to use it
- The exact memo template/structure the output should follow
- A set of instructions (e.g. don't invent facts that weren't in the original notes, keep bullet points action-oriented, keep the memo under a page)
- A worked example showing sample input notes and the expected formatted output

When an AI assistant (in my case, Cline connected to MindRouter) is told to use this skill on a set of notes, it reads `SKILL.md`, follows the format and rules defined there, and produces a memo in the standard structure — without me having to re-explain the format every single time.

I tested it by asking Cline to format two different sets of rough notes into memos, and it correctly followed the template, used placeholders for information I hadn't provided (like sender name and date), and flagged that I should fill those in before distributing.

## Why I Created This Skill

Business memos come up constantly in real workplaces, but writing one from scratch every time — getting the header block right, deciding what goes in Background vs. Purpose, making sure Next Steps are actually actionable — is repetitive and easy to get inconsistent. A skill lets me encode that format once and reuse it any time I have rough notes that need to become a formal memo, which is exactly the kind of "reusable instructions for a repeated task" this week's lecture described.

## How This Could Be Useful Later

Any time I (or a team I'm on) need to turn meeting notes, a Slack thread, or a quick brain dump into something formal and shareable, this skill removes the friction of remembering the right structure. It could also be adapted for other class assignments or internship/work tasks — the same pattern (a template + rules + an example) could be turned into skills for weekly status reports, project update emails, or any other document type I need to produce repeatedly and consistently.