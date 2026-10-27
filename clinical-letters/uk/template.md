# Templates: PRSB Outpatient Letter and eDischarge Summary

Heading names are PRSB verbatim. Tag = conformance in that standard
(M mandatory, R required, O optional). Order is this skill's default; PRSB
leaves order to local agreement. Drop R and O headings that have no content.
Never drop an M heading. Placeholders in <angle brackets>.

## A. Outpatient Letter (PRSB v2.2) — use for clinic, telephone and video consultations

<Hospital / Trust name>, <Department or clinic>
<Letter date DD-Mon-YYYY>
Dear Dr <GP surname>,

### Patient demographics [M]
<Full name>; Date of birth <DD-Mon-YYYY>; NHS number <000 000 0000>; Gender <...>; Address <...>; Telephone <...>
Rule: name, DOB, address always; NHS number or "not known"; no bare hospital number.

### GP practice [M]
<Practice name, address, practice code>; Usual GP <Dr ...>
Rule: write "No known GP practice" if unregistered.

### Referrer details [R]
<Name, role, organisation> or "Self-referral"
Rule: must be present in a first-appointment letter.

### Attendance details [M]
Date and time of contact <DD-Mon-YYYY HH:MM>; Contact type <first / follow-up>; Consultation method <face to face / telephone / video>; Specialty <...> or Service <...>; Responsible healthcare professional <name, role>; Seen by <name, role>; Person accompanying <...>; Outcome of outpatient attendance <discharged to GP / follow-up in <n> weeks / ...>
Rule: one of Specialty or Service; follow-up appointments go here, not in Plan.

### Diagnoses [R]
1. <Primary diagnosis or symptom> (SNOMED CT <code>) — <stage, comment>
2. <Comorbidity>
Rule: highest-certainty concept; differentials only as free-text comment.

### Problems and issues [R]
<Significant findings, symptoms or signs not yet a diagnosis>

### Clinical summary [M]
<Two to six sentences: why seen, what was found, what it means, any patient disagreement, any reason the patient is not copied>

### History [R]
Reason for referral <...>; Presenting complaints <...>; History of each complaint <...>; History since last contact <...>; Relevant past medical, surgical and mental health history <...>
Rule: full at first appointment; only "history since last contact" at follow-up.

### Examination finding [O]
<Pertinent findings; BP <n/n> mmHg, pulse <n>/min, weight <n> kg, BMI <n> kg/m²>

### Investigation results [O]
<Test, date, result with UK unit, interpretation>; Pending: <test, who will act on it>

### Procedures [R]
<Procedure actually performed, date, outcome; medicines given in clinic>

### Medications and Medical Devices [O]
| Medicine (dm+d product) | Dose directions | Status | Reason for medication / change | Duration |
| <Name strength form> | <take ... > | Added / Amended / Discontinued | <reason> | <continue indefinitely / n days> |
Rule: changes only; if none write "No changes to the patient's regular medication".

### Allergies and adverse reactions [M]
<Causative agent — reaction, severity, certainty> or "No known drug allergies or adverse reactions" or "Information not available"

### Plan and requested actions [R]
Actions for the GP: <action, by when>
Actions for the patient or carer: <action>
Actions for the clinic: <action>
Agreed with patient or legitimate representative: <yes / no / partly>
Rule: every action names who does it and when; phrase GP actions as requests.

### Information and advice given [R]
<What was explained, to whom; leaflet named, not reproduced>

### Patient and carer concerns, expectations and wishes [O]
<In their words>

### Individual requirements [R]
<Language, interpreter, communication, mobility, cultural needs>

### Social context [O] / Family history [O] / Clinical review of systems [O] / Assessment scales [O] / Relevant clinical risk factors [O]
<Only if it changes care>

### Legal information [R]
<Consent, mental capacity assessment and the decision it relates to, LPA, ADRT, safeguarding>

### Safety alerts [R]
<Risks to self or others>

### Participation in research [R]
<Drug or intervention, trial name, currently enrolled yes/no>

### Person completing record [M]
<Name>, <role and grade>, <specialty>, <GMC or HCPC number>; Date and time completed <DD-Mon-YYYY HH:MM>; Contact <telephone or NHS email>

### Distribution list [R]
1. Patient copy — <name>
2. <Other recipient: name, role, organisation>

Yours sincerely,
<Name, role>

## B. eDischarge Summary (PRSB v2.1) — use for inpatient, day-case and A&E discharge

Same header, salutation, style and tags convention. Differences from A: no
Attendance details, History, Problems and issues, Family history, Clinical
review of systems, Examination finding, Relevant clinical risk factors; adds
Admission details and Discharge details; Diagnoses becomes M; Procedures,
Participation in research become O; Patient and carer concerns becomes R.

### Patient demographics [M]  — as A
### GP practice [M]  — as A
### Referrer details [R]  — as A
### Admission details [R]
Date/time of admission <...>; Admission method <elective / emergency>; Source of admission <home / ...>; Reason for admission <...>
### Discharge details [R]
Date/time of discharge <...>; Discharge method <...>; Discharge destination <...>; Discharging consultant <...>; Discharging specialty/department <...>
### Diagnoses [M]
<Primary first; new diagnoses made during admission; symptom if none>
### Procedures [O]
<All clinically important procedures actually done, with dates and outcomes>
### Clinical summary [M]
<Brief course of the admission and condition at discharge; important inactive history as narrative>
### Investigation results [O]  — as A, pending results listed
### Assessment scale [O]
<Scale, score, date>
### Medications and Medical Devices [O]
| Medicine (dm+d product) | Dose directions | Status | Reason | Duration | Quantity supplied (prescribed / dispensed) |
Rule: list Continued, Added, Amended and Discontinued admission medicines with reasons; omit drugs both started and stopped in hospital.
### Allergies and adverse reactions [M]  — as A
### Patient and carer concerns, expectations and wishes [R]
### Information and advice given [R]  — as A
### Plan and requested actions [R]  — as A; name who follows up each pending result
### Individual requirements [R] / Social context [O] / Legal information [R] / Safety alerts [R] / Participation in research [O]
### Person completing record [M]  — as A
### Distribution list [R]  — patient first
