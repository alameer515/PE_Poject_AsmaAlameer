# Library Index

| Template | Task | Variables | Version | Status |
|---|---|---|---|---|
| [LB-Answer-Question](templates/LB-Answer-Question-v1_2026_10_15.md) | Answer beneficiary or client questions with factual consistency | `[QUESTION]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[DESK_FACTS]` | v1 | Ready to demo |
| [LB-Friendly-StaffNote](templates/LB-Friendly-StaffNote-v1_2026_10_15.md) | Draft a friendly, clear internal note for staff collaboration | `[TOPIC]` `[RECIPIENT]` `[LANGUAGE]` `[KEY_POINTS]` | v1 | Ready to demo |
| [LB-Reminder-DueDate](templates/LB-Reminder-DueDate-v1_2026_10_15.md) | Send a clear reminder notification regarding upcoming due dates | `[RECIPIENT]` `[TASK_NAME]` `[DUE_DATE]` `[LANGUAGE]` `[TONE]` | v1 | Ready to demo |
| [LB-Sort-Request](templates/LB-Sort-Request-v1_2026_10_15.md) | Classify and route incoming requests to the appropriate department | `[REQUEST]` `[CATEGORIES]` `[LANGUAGE]` | v1 | Ready to demo |
| [LB-Summary-Letter](templates/LB-Summary-Letter-v1_2026_10_15.md) | Summarize incoming correspondence or letters for team review | `[LETTER_TEXT]` `[LANGUAGE]` `[MAX_WORDS]` `[FOCUS]` | v1 | Ready to demo |

## Shared blocks

| Block | Used by | File |
|---|---|---|
| Desk facts (v1) | LB-Answer-Question | `blocks/DeskFacts-v1_2026_10_15.md` |

## Rules

| File | What it is |
|---|---|
| `rules/Desk-Rules-v1_2026_10_15.md` | Five responsible-use rules (example set; replace with your own) |

## Archive

Older versions stay in the `_archive` folders so the library keeps its history:
- no files

## `[LANGUAGE]` values (same in every template)

| Value | Meaning |
|---|---|
| Arabic | Answer in Arabic only |
| English | Answer in English only |
| Automated | Reply in the main language of the inquiry |
| Bilingual | Two separate versions: Arabic, then English |
| Mixed | One reply that merges Arabic and English |

## Change log

| Date | Change |
|---|---|
| 2026_10_15 | Library overhaul: LB templates (Answer-Question, Friendly-StaffNote, Reminder-DueDate, Sort-Request, Summary-Letter); updated DeskFacts and Desk-Rules to 2026_10_15 |