---
name: clinical-letter-core
description: Shared rules for any letter from a hospital doctor to a patient's general practitioner, in any country. Use together with the country skill (dk-epikrise, nl-ontslagbericht-hasp, de-arztbrief, uk-prsb-clinical-letter, fr-lettre-de-liaison). Read this first, then the country skill, its template.md, and its checklist.md before finishing.
---

# Clinical letter core

These rules apply in every country. The country skill decides structure,
headings, language and local conventions. When the two disagree on structure,
the country skill wins. When the two disagree on truthfulness or safety, this
skill wins.

## How to work

1. Read the country skill named in the task. If the task names a country but no
   skill matches, say so in the letter header and fall back to the most
   similar skill, naming which one you used.
2. Read the country skill's `template.md` and build the letter on that
   skeleton. Do not invent headings and do not reorder them.
3. Retrieve the record before writing. Every clinical statement must trace to
   a resource you read: a problem, a lab, a note, a medication order. Do not
   write from memory of the task text alone.
4. Before finishing, read the country skill's `checklist.md` and walk every
   item. Fix the letter, not the checklist.

## Grounding

- State only what the record supports. If a value or a date is missing,
  write "not recorded" rather than a plausible guess.
- Quote numeric results with the unit and the date they were taken.
- Convert units to the destination country's convention when the country skill
  says so, and keep the original value in parentheses the first time.
- Never copy an entire source note. Summarise what the GP needs.
- Do not include identifiers the destination country does not use (for
  example a US MRN in a Danish letter). Use the identifier scheme the country
  skill names, or "identifier: see record" if none applies.

## Medication changes

Describe every change as one of exactly four states, in the country skill's
language: started, stopped, changed, continued. For started and changed give
the indication. For stopped give the reason. Give dose, route, frequency and,
where known, duration. Name the substance (generic or INN) first; a brand name
may follow in parentheses if the record uses it.

## Follow-up and safety

- Say who does what and by when. A recommendation without an owner or a time is
  incomplete.
- Pending results: name them and say who will act on them.
- Safety-critical facts (allergies, anticoagulation, immunosuppression,
  resistant organisms, implanted devices, treatment limits) go where the
  country skill places them and are never omitted for brevity.

## Register and length

- Write for a busy GP: short sentences, no specialty jargon unless the country
  skill allows it, abbreviations expanded on first use.
- One letter, one recipient. If a copy goes to the patient, write so the
  patient can read it too.
- Aim for the length a GP can read in two minutes. The country skill's
  example.md shows the target.

## What not to do

- No speculation presented as fact. Mark differential or uncertain items as
  such.
- No instructions to the GP that the hospital should carry out itself.
- No placeholder text left in the final letter.
- No content outside the template's headings.

## Self-check

Open the country skill's `checklist.md` and confirm each item. Then confirm
these four:

1. Every clinical statement traces to a retrieved resource.
2. Every medication appears with one of the four states.
3. Every recommendation has an owner and a time.
4. No heading is missing, added, or out of order relative to `template.md`.
