# Terminology: PRSB headings, code systems, units, dates, abbreviations

Heading definitions are the "Description" text of the PRSB information models
(Outpatient Letter v2.2, 6 Apr 2023; eDischarge Summary v2.1, 1 Feb 2021),
shortened. OP/eDS = conformance in each standard (M/R/O, "-" = absent).

## PRSB headings and definitions

| Heading | OP | eDS | Definition |
|---|---|---|---|
| Patient demographics | M | M | Patient details and contact information |
| GP practice | M | M | Details of the GP practice where the patient is registered |
| Referrer details | R | R | Individual or team who referred the patient |
| Attendance details | M | - | The details of the patient contact (date/time, method, specialty or service, responsible professional, seen by, outcome) |
| Admission details | - | R | Details of the admission and reason for admission |
| Discharge details | - | R | Details of the discharge from hospital |
| History | R | - | Development of each presenting complaint and the patient's relevant health history |
| Social context | O | O | Household, occupational history, lifestyle factors |
| Family history | O | - | Illness in family relations relevant to the patient's care |
| Clinical review of systems | O | - | Symptoms related to physiological systems |
| Examination finding | O | - | Findings from clinical examination |
| Assessment scales (eDS: Assessment scale) | O | O | Any assessment scales used |
| Diagnoses | R | M | A list of the patient's diagnoses |
| Problems and issues | R | - | Problems that require investigation or treatment |
| Relevant clinical risk factors | O | - | Risk of clinical deterioration, risk factors, mitigation plans |
| Clinical summary | M | M | A brief description of the encounter |
| Investigation results | O | O | Investigations and procedures requested, results and plans |
| Procedures | R | O | Any procedures performed |
| Medications and Medical Devices | O | O | Medications and medical equipment the patient is using, with instructions |
| Allergies and adverse reactions | M | M | Known allergies, intolerances or adverse reactions |
| Legal information | R | R | Consent to treatment, mental capacity, and similar |
| Safety alerts | R | R | Risks the patient poses to themselves or others |
| Patient and carer concerns, expectations and wishes | O | R | Concerns, expectations or wishes of the patient (or carer) |
| Information and advice given | R | R | Information or advice given to patient, carer or third party |
| Plan and requested actions | R | R | Planned investigations, procedures and treatment, and whether agreed with the patient |
| Participation in research | R | O | Research studies participated in |
| Person completing record | M | M | The person who filled out the record |
| Distribution list | R | R | Other individuals to receive a copy of this communication |

## Medication status vocabulary (eDS model, Medication change summary)

Continued = present on admission and discharge, unchanged. Added = on discharge,
not on admission. Amended = present on both, changed (drug, dose, form,
strength). Discontinued = on admission, stopped (eDS "Medication discontinued
entry"). Duration terms: "Continue indefinitely" (ongoing treatment planned,
e.g. a statin); "Do not discontinue" (sudden stopping is dangerous, e.g.
long-term steroids). Display "indication" as "reason for medication" or "reason
for medication change".

## Code systems and identifiers

| Item | Use in the letter |
|---|---|
| SNOMED CT | Diagnoses, problems, procedures, allergy causative agents: term then code, e.g. "Type 2 diabetes mellitus (SNOMED CT 44054006)" |
| dm+d (NHS dictionary of medicines and devices) | Medicine names: product (VMP/AMP, "Ramipril 2.5 mg capsules") or drug (VTM, "Ramipril") |
| NHS number | 10 digits, displayed 000 000 0000; "not known" if unavailable; CHI number equivalent in Scotland |
| GMC / HCPC / NMC number | Professional identifier of the person completing the record |
| ODS practice code | Optional GP practice identifier (e.g. Y99901) |
| Not used | ICD-10, OPCS-4, Read codes, US CPT or ICD-10-CM |

## Units (UK laboratory convention, skill default) and conversions

| Measure | UK unit | From US |
|---|---|---|
| Glucose | mmol/L | mg/dL ÷ 18 |
| HbA1c | mmol/mol (IFCC) | % × 10.93 − 23.5 |
| Cholesterol (total, LDL, HDL, non-HDL) | mmol/L | mg/dL ÷ 38.67 |
| Triglycerides | mmol/L | mg/dL ÷ 88.57 |
| Creatinine | µmol/L | mg/dL × 88.4 |
| eGFR | mL/min/1.73m² | same |
| Haemoglobin | g/L | g/dL × 10 |
| Potassium, sodium | mmol/L | mEq/L (same number) |
| Blood pressure | mmHg | same |
| Weight, height, BMI | kg, cm or m, kg/m² | lb ÷ 2.205; in × 2.54 |
| Temperature | °C | (°F − 32) × 5/9 |

## Dates and times

DD-Mon-YYYY (14-Oct-2026), 24-hour clock (10:20). Never US month-first order.
Give full dates for attendance, admission, discharge, tests, medication
start/stop, and completion of the record.

## Abbreviations: expand on first use

Permitted unexpanded: NHS, GP, SNOMED CT, dm+d, BMI after first expansion.

| Short | Write |
|---|---|
| A&E / ED | emergency department |
| ACEi / ARB | ACE inhibitor (angiotensin-converting enzyme inhibitor) / angiotensin receptor blocker |
| AF | atrial fibrillation |
| AHP | allied health professional |
| ADRT / LPA | advance decision to refuse treatment / lasting power of attorney |
| BD / TDS / QDS / OD / ON / PRN | twice a day / three times a day / four times a day / once daily / at night / when required |
| BP / HR / RR / SpO2 | blood pressure / heart rate / respiratory rate / oxygen saturation |
| CKD | chronic kidney disease |
| COPD | chronic obstructive pulmonary disease |
| CT / MRI / CXR / ECG / Echo | CT scan / MRI scan / chest X-ray / electrocardiogram / echocardiogram |
| DNA | did not attend |
| DOAC | direct oral anticoagulant |
| DVT / PE | deep vein thrombosis / pulmonary embolism |
| FBC / U&E / LFT / TFT / CRP | full blood count / urea and electrolytes / liver function tests / thyroid function tests / C-reactive protein |
| GORD | gastro-oesophageal reflux disease |
| HbA1c | glycated haemoglobin (HbA1c) |
| HF / IHD / MI | heart failure / ischaemic heart disease / myocardial infarction (heart attack) |
| MDT | multidisciplinary team |
| NAD | no abnormality detected |
| NKDA | write "No known drug allergies or adverse reactions" |
| NSAID | non-steroidal anti-inflammatory drug |
| OPD / OPA / F/U | outpatient department / outpatient appointment / follow-up |
| PMH / DH / SH / FH | past medical history / drug history / social history / family history |
| PO / IV / IM / SC | by mouth / intravenous / intramuscular / subcutaneous |
| PPI | proton pump inhibitor |
| SGLT2i | SGLT2 inhibitor (sodium-glucose co-transporter-2 inhibitor) |
| SOB / SOBOE | shortness of breath / shortness of breath on exertion |
| T2DM / T1DM | type 2 diabetes / type 1 diabetes |
| TCI / SOS | to come in / open appointment on request |
| TIA / CVA | transient ischaemic attack / stroke |
| UTI | urinary tract infection |
| # / Dx / Rx / Ix / Mx | fracture / diagnosis / treatment / investigations / management |
