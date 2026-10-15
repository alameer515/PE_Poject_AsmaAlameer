# Member Services Desk — Prompt Library (Day 5)
مكتبة أوامر مكتب خدمات الأعضاء — المكتبة العامة

A standardized set of tested prompt templates for Scenario B5 (Public Library Member Services Desk). Desk agents draft responses, and a librarian reviews and approves each output before sending.

## What is inside

| Path | What it is |
|---|---|
| `00_Library_Index.md` | The master list of templates, tasks, variables, and versions |
| `templates/` | One file per template (5 active templates based on the standard skeleton) |
| `blocks/DeskFacts-v1_2026_10_15.md` | The 7 official Library Facts injected into `[DESK_FACTS]` |
| `rules/Desk-Rules-v1_2026_10_15.md` | Responsible-use rules, safety protocols, and data privacy policies |
| `_archive/` folders | Older templates and blocks preserved for change history |
| `templates/_BLANK_ENTRY.md` | Reusable blank template skeleton for adding new tasks |

## The daily habit: Pick, Fill, Run, Review

1. **Pick** the appropriate `LB-` template from `00_Library_Index.md`.
2. **Fill** all `[VARIABLE]` placeholders. **Mask first**: replace all real names, membership numbers, and contact details with placeholders (e.g., `Member-1`, `Card-X`, `Phone-1`).
3. **Run** the prompt with your chosen AI tool.
4. **Review**: A human librarian must verify every output against the official Library Facts before release.
5. **Verify**: Ensure the response contains no hallucinated dates, actions, or sensitive requests (passwords, PINs, bank details), and delete internal review markers before sending.

## Naming rule

`LB-<Task>-<Object>-v<number>_<yyyy_mm_dd>`
Example: `LB-Answer-Question-v1_2026_10_15.md`

## Library rules

- **Strict Source Grounding**: Rely only on provided facts. If information is unavailable, explicitly state so and direct members to the library app or desk.
- **Data Privacy**: Never collect or repeat personal identification numbers, passwords, or banking information.
- **Human in the Loop**: No AI-generated output is sent directly to a library member without librarian sign-off.
- **Version Control**: Every change is versioned; deprecated files are archived in `_archive/` without deletion.

## Core Library Facts (Summary)

1. Working hours: Saturday to Thursday, 09:00 to 20:00.
2. Borrowing period: 14 days per book.
3. Loan renewals: Up to 2 times, at least 1 day before the due date.
4. Card replacement: Handled in person at the desk.
5. Live reservation queue: Not accessible to the desk; refer member to the library app.
6. Inquiry response SLA: Within 2 working days.
7. Data sensitivity: The desk never asks for ID numbers, passwords, or bank details.

## About the examples

All example fills and model outputs provided in the templates are synthetic and use masked variables. Output style may vary between model architectures; evaluate outputs against the checklist rather than verbatim matching.