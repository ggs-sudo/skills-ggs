# Checklist: PRSB hospital-to-GP letter (England)

Each line is pass/fail. Tags: [structure] [content] [style] [forbidden].
Run part A, then part B or C depending on the letter type.

## A. All letters

1. [structure] Exactly one standard used: all headings are from the Outpatient Letter set or all from the eDischarge set, none from both.
2. [structure] Every heading is spelt exactly as PRSB names it (e.g. "Medications and Medical Devices", "Allergies and adverse reactions", "Plan and requested actions").
3. [structure] Headings appear in the template.md default order (or the local order the task gave).
4. [structure] No heading is present with empty, "N/A", "nil" or "none recorded" content, except Allergies and adverse reactions (fixed wording) and Medications and Medical Devices ("No changes to the patient's regular medication").
5. [structure] Patient demographics present with full name, date of birth, address and NHS number (or "NHS number not known").
6. [structure] GP practice present with practice name and address, or "No known GP practice".
7. [structure] Clinical summary present and no longer than about six sentences.
8. [structure] Allergies and adverse reactions present and is either a list of agent plus reaction, or exactly "No known drug allergies or adverse reactions", or exactly "Information not available".
9. [structure] Person completing record present with name, role, GMC/HCPC/NMC number, date and time completed, and a contact telephone or email.
10. [structure] Distribution list present and lists the patient (or Clinical summary explains why the patient is not copied).
11. [content] Diagnoses lists the primary diagnosis first and names a symptom when no diagnosis is established.
12. [content] No differential, suspected or excluded diagnosis is presented as a diagnosis entry; such reasoning appears only as free-text comment.
13. [content] Each diagnosis is given as a SNOMED CT term (code in brackets where known); no ICD-10 or OPCS codes anywhere.
14. [content] Medication table rows each have name (dm+d product or drug), dose directions, status (Added / Amended / Discontinued / Continued), and a reason.
15. [content] Every Plan action names who is responsible (GP, patient or carer, clinic) and a time frame; GP actions are phrased as requests ("Please ...").
16. [content] Plan states whether it was agreed with the patient or legitimate representative.
17. [content] Investigation results give date, value and UK unit for each result and say who will act on any pending result.
18. [content] Information and advice given names any leaflet without reproducing its content.
19. [content] Every statement in the letter can be traced to the source record; nothing invented (values, dates, identifiers, names).
20. [style] Written in plain English a patient can follow; British spelling; formal letter register with salutation to the GP and sign-off.
21. [style] Every abbreviation other than NHS, GP, SNOMED CT, dm+d (and BMI after expansion) is expanded on first use.
22. [style] Dates are DD-Mon-YYYY and times 24-hour; no US month-first dates.
23. [style] Laboratory values in UK units (mmol/L, mmol/mol for HbA1c, µmol/L creatinine, g/L haemoglobin); US values converted.
24. [style] The word "indication" is not used; "reason for medication" or "reason for medication change" is.
25. [forbidden] No heading or label from another national format (Kern, Epikrise, Entlassbrief, Hospital Course, Anamnese, Beleid).
26. [forbidden] Letter is not called provisional, interim, preliminary or "brief summary", and does not promise a later fuller letter.
27. [forbidden] No bare hospital number without the issuing organisation named.
28. [forbidden] No real patient data; identifiers are the task's or synthetic.

## B. Outpatient Letter (PRSB v2.2) additions

29. [structure] All six mandatory headings present: Patient demographics, GP practice, Attendance details, Allergies and adverse reactions, Clinical summary, Person completing record.
30. [structure] Attendance details gives date and time of contact, responsible healthcare professional, seen by, consultation method, and Specialty or Service.
31. [structure] Attendance details states the outcome of the attendance (discharged to GP, follow-up interval, or awaiting results); follow-up appointments are not placed under Plan and requested actions.
32. [structure] For a first appointment: Referrer details and History (reason for referral, presenting complaints, relevant past history) are present.
33. [structure] Diagnoses and Problems and issues both present when information exists; findings that are not a diagnosis sit under Problems and issues.
34. [content] Medications and Medical Devices lists only medicines added, amended or discontinued at this attendance, with reasons, or the single line "No changes to the patient's regular medication"; unchanged regular medicines are not listed.
35. [content] Medicines administered in clinic appear under Procedures, not under Medications and Medical Devices.
36. [content] No Admission details or Discharge details heading.
37. [content] Letter date is within 7 days of the attendance date.

## C. eDischarge Summary (PRSB v2.1) additions

38. [structure] All six mandatory headings present: Patient demographics, GP practice, Diagnoses, Clinical summary, Allergies and adverse reactions, Person completing record.
39. [structure] Admission details (date/time, method, source, reason for admission) and Discharge details (date/time, method, destination, discharging consultant and specialty) present.
40. [structure] No Attendance details, History, Problems and issues, Examination finding, Family history or Clinical review of systems heading.
41. [content] Medications and Medical Devices lists continued, added, amended and discontinued admission medicines with reasons; drugs both started and stopped in hospital are not listed; quantity supplied and prescribed/dispensed stated where known.
42. [content] Procedures lists what was actually done with dates and outcomes, not the planned procedure.
43. [content] Clinical summary describes the course of the admission and condition at discharge, including clinically important inactive history as narrative.
44. [content] Patient and carer concerns, expectations and wishes present when any were recorded (required in eDS).
45. [content] Letter date is within 24 hours of the discharge date and time.
