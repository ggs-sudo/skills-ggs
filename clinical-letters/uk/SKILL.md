---
name: uk-prsb-clinical-letter
description: Write the NHS hospital letter to the patient's GP practice in the UK (England) in the PRSB structure, either the Outpatient Letter (specialist clinic consultation) or the eDischarge Summary (inpatient discharge). Use for any letter to the GP in the UK, NHS discharge summary, outpatient or clinic letter, or PRSB headings. Read template.md for heading order and checklist.md before finishing.
---

# uk-prsb-clinical-letter: hospital-to-GP letter, England

Sources read (cited in brackets): PRSB Outpatient Letter Standard v2.2 model,
6 Apr 2023 [OP-xlsx]; its Implementation Guidance Report, 2018 [OP-G §]; PRSB
eDischarge Summary Standard v2.1 model, 1 Feb 2021 [eDS-xlsx]; its Implementation
Guidance v2.1, Jan 2019 [eDS-G §]; NHS Standard Contract 2024/25 Service
Conditions [SC11]. Both standards pass to NHS England on 1 Jan 2026 under OGL v3.
"(skill default)" marks this skill's choice, not a rule of the standard.

Workflow: 1) this file; 2) build on [template.md](template.md); 3) terms in
[terminology.md](terminology.md); 4) register of [example.md](example.md);
5) run [checklist.md](checklist.md) before finishing.

## 1. Scope: which standard

- Clinic, telephone or video consultation without admission, first or
  follow-up, by doctor, nurse or AHP: **Outpatient Letter** [OP-G 4.1.2], sent to
  the GP and copied to the patient [OP-G 4.1.1].
- Discharge after inpatient, day-case or A&E episode: **eDischarge Summary**
  [eDS-G 4.1.2; SC11.5]. Never mix the two heading sets.
- One letter per episode: "a single outpatient letter, containing all pertinent
  information" [OP-G 4.1.6]; "sending an initial brief summary and following up
  with a later more detailed letter should be deprecated" [eDS-G 4.1.4].
- Timing (contract, not PRSB): Discharge Summary "within 24 hours following that
  transfer or discharge" [SC11.5]; Clinic Letter "as soon as reasonably
  practicable and in any event within 7 days" of the attendance [SC11.7].

## 2. Headings and conformance

[OP-G 3.2; eDS-G 3.2]: "MANDATORY sections must always be included";
"REQUIRED: if there is information recorded it should be sent"; "OPTIONAL: a
local decision"; M and R "should not be 'downgraded'". Empty sections "should
be excluded" (Allergies excepted, see table). Use PRSB heading names verbatim.
OP = Outpatient Letter v2.2, eDS = eDischarge v2.1, "-" = absent from that
standard. Heading definitions are in [terminology.md](terminology.md).

| Heading | OP | eDS | Rule |
|---|---|---|---|
| Patient demographics | M | M | Name, DOB, address; NHS number (§5); no bare hospital number [eDS-G 3.4.3] |
| GP practice | M | M | Practice name and address; else "No known GP practice" [OP-G 3.5.4] |
| Referrer details | R | R | Required in a first-appointment letter [OP-G 4.3.1]; "self-referral" if none |
| Attendance details | M | - | Date/time, responsible professional, seen by, Specialty or Service, outcome; follow-up appointments go HERE, not in Plan [OP-G 4.6, 4.16.2] |
| Admission details | - | R | Date/time, method, source, reason for admission |
| Discharge details | - | R | Date/time, method, destination, discharging consultant, specialty |
| History | R | - | Referral reason, complaints and past history at a first appointment; history since last contact at follow-up [OP-G 4.12] |
| Social context | O | O | Only if it changes care |
| Family history | O | - | Only if relevant |
| Clinical review of systems | O | - | Rare |
| Examination finding | O | - | Pertinent findings, vital signs with units |
| Assessment scales | O | O | Scale, score, date (eDS spells it "Assessment scale") |
| Diagnoses | R | M | Highest-certainty concept, or the symptom if none; differentials as free text only; comorbidities separate; primary first [OP-G/eDS-G 4.4] |
| Problems and issues | R | - | Significant findings not yet a diagnosis [OP-G 4.13.1] |
| Relevant clinical risk factors | O | - | Deterioration risk and mitigation |
| Clinical summary | M | M | "Where possible, very brief"; your opinion; any patient disagreement; why no patient copy if none [OP-G 4.16.3, 4.17.3] |
| Investigation results | O | O | Only what the GP must see; why done, who follows up; pending tests [OP-G 4.11] |
| Procedures | R | O | Procedures actually done; medicines given in clinic (OP) [OP-G 4.5.1, 4.9.3]; no OPCS codes [4.5.5] |
| Medications and Medical Devices | O | O | §6; include whenever any medicine changed (skill default) |
| Allergies and adverse reactions | M | M | Agent and reaction; else exactly "No known drug allergies or adverse reactions" or "Information not available" [OP-G 4.10.3] |
| Legal information | R | R | Consent, mental capacity per decision, LPA, ADRT, safeguarding [eDS-G 4.12] |
| Safety alerts | R | R | Risks to self or others [OP-G 4.8] |
| Patient and carer concerns, expectations and wishes | O | R | In their words |
| Information and advice given | R | R | Concise; name a leaflet, do not reproduce it [OP-G 4.17.2] |
| Plan and requested actions | R | R | Every action names who and by when; state whether it was agreed with the patient [OP-G 4.16.1] |
| Participation in research | R | O | Drug or intervention, trial name, currently enrolled [OP-G 4.14] |
| Person completing record | M | M | Name, role, GMC/HCPC number, date and time completed; contact for queries [OP-xlsx] |
| Distribution list | R | R | Every copy recipient, patient first [OP-xlsx] |

## 3. Heading order

"The order in which headings appear can be agreed locally" [OP-G 3.1.2; eDS-G
3.1.2]; the standards are "a common structure to the record, not a style guide"
[3.1.5]. This skill's default order is the one in [template.md](template.md). Keep it
unless the task gives a local order.

## 4. Style

- "Communications should be brief, where possible, containing only pertinent
  information", not duplicating what the GP holds [OP-G 3.1.12].
- The patient is copied by default, so write to be "understandable to the
  general public" without losing precision [OP-G 3.1.14; eDS-G 3.1.15]: plain
  English, short sentences, British spelling, formal register ("Dear Dr X",
  "Yours sincerely"), the patient named rather than "the patient" throughout.
- Expand every abbreviation on first use except NHS, GP, SNOMED CT and dm+d.
  Write "reason for medication" and "reason for medication change", never
  "indication" [OP-G 4.9.15].
- Name the source when information came from a relative or agency [OP-G 3.1.8].

## 5. Coding, identifiers, units, dates

- SNOMED CT for diagnoses, procedures, allergies; dm+d for medicines and devices
  [OP-G 3.3.1]; term first, code in brackets where known, "coded data ...
  carried with the associated text" [3.1.16]. No ICD-10, no OPCS [OP-G 4.5.5].
- NHS number mandatory "with the option to record not known or not available"
  [eDS-G 3.4.1]; 10 digits shown 000 000 0000 (skill default; NHS Data
  Dictionary not read).
- Dates DD-Mon-YYYY, 24-hour times (skill default; standards fix no format).
- UK units (skill default): mmol/L glucose, lipids, electrolytes; mmol/mol
  HbA1c; µmol/L creatinine; mL/min/1.73m² eGFR; g/L haemoglobin; mmHg; kg, cm,
  kg/m². Convert US values (mg/dL, %).

## 6. Medications and Medical Devices

- Outpatient: only medicines changed, discontinued or added at the attendance,
  each with its reason [OP-G 4.9.1-2]; NOT unchanged continuing medicines, NOT
  drugs given in clinic [4.9.3]; if nothing changed: "No changes to the
  patient's regular medication" [4.9.10].
- Discharge: continued, amended, discontinued and new medicines with reasons
  [eDS-G 4.9.1]; omit drugs both started and stopped in hospital [4.9.2];
  quantity supplied, prescribed or dispensed [4.9.11].
- Per item: dm+d product plus dose directions ("Furosemide 40 mg tablets, take
  2 at 8am") or drug, dose amount, route, timing [OP-G 4.9.23]; status
  Continued / Added / Amended / Discontinued [eDS-xlsx]; reason; duration with
  "continue indefinitely" or "do not discontinue" as defined [OP-G 4.9.6].
- Any change needing a new GP prescription is "Amended" [4.9.7]; GP record
  changes "MUST always require the authorisation of the responsible GP
  prescriber" [4.9.19], so GP actions are requests, not orders.

## 7. Forbidden

Headings from other national formats (Kern, Epikrise, Entlassbrief, Hospital
Course); mixed OP and eDS heading sets; blank or "N/A" headings; "provisional",
"interim", "full letter to follow"; coded differential or excluded diagnoses;
OPCS or ICD-10 codes; invented identifiers, dates or results; US units;
unexpanded abbreviations; a missing patient copy with no explanation.

## 8. Header metadata

Letter date; attendance (or admission and discharge) date and time; specialty
or service; responsible clinician; NHS number; GP practice; patient in
Distribution list; author name, role, GMC/HCPC number, date and time completed,
contact telephone or NHS email [OP-xlsx].

## 9. Self-check

Open [checklist.md](checklist.md), confirm every line, fix, then finish.

## 10. Sources read

`OP-xlsx` PRSB Outpatient Letter Standard v2.2 information model, 6 Apr 2023.
`OP-G` its implementation guidance, 2018, by section (predates v2.2).
`eDS-xlsx` PRSB eDischarge Summary Standard v2.1 model, 1 Feb 2021 (matches
the NHS ITK FHIR heading table). `eDS-G` its guidance report v2.1, Jan 2019.
`SC11` NHS Standard Contract 2024/25 Service Conditions: SC11.5 discharge
summary within 24 h, SC11.7 clinic letter within 7 days — contractual, not
PRSB. Both standards pass to NHS England on 1 Jan 2026. Conflict: OP-G 4.18
calls Distribution list Optional, the v2.2 model requires it; follow v2.2.
