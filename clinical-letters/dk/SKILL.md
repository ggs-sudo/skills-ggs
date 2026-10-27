---
name: dk-epikrise
description: Write the epikrise, the Danish hospital letter to the patient's own GP (egen læge), for a patient treated at a Danish hospital in Denmark, following Styrelsen for Patientsikkerhed's Vejledning om epikriser (VEJ 10036). Use for any letter to the GP in Denmark, discharge or ambulatory. Read template.md for heading order and checklist.md before finishing.
---

# dk-epikrise: letter to the GP in Denmark

Rules come from STPS "Vejledning om epikriser", VEJ nr 10036 af 30/11/2018, in
force 1 July 2019 (cited §). Colour marking from Danske Regioner, "Faglig
vejledning vedr. styrket opfølgningsindsats i almen praksis", 30-04-2019 (cited
DR). (konvention) = common practice, not in the vejledning. (UNVERIFIED) = no
primary source read.

Workflow: read this file; build on [template.md](template.md); check terms in
[terminology.md](terminology.md); compare register with [example.md](example.md);
run [checklist.md](checklist.md) before finishing.

## 1. Scope and addressee

- Epikrise = "en skriftlig overlevering af lægefaglige oplysninger fra en læge
  til en anden læge" at discharge or any other end of a course, including
  "ambulant behandling, lægevagt, akutmodtagelser" (§1, §2).
- "Patientens egen læge er primær modtager" (§4.3.1). A copy may go to the
  referring praktiserende speciallæge or vagtlæge "til orientering, læring og
  kvalitetssikring" (§4.2.2); copy recipients get no follow-up duty (§4.3.2).
- Ward or hospital transfer takes an overflytningsnotat, not an epikrise (§1).
- The doctor responsible for content and marking cannot delegate it (§4.2).
- To the GP: "Der er alene tale om anbefalinger, ikke overdragelse af opgaver"
  (§2.2). Write "anbefales", never orders.

## 2. Required sections, in order

Fixed by the vejledning: follow-up recommendation "skal ... stå i begyndelsen
af epikrisen" (§2.2); medication list "skal indsættes i overskuelig form til
sidst i epikrisen" (§2.8). Sections 3 to 7 follow the vejledning's own
numbering (konvention). Use the Danish headings verbatim.

1. **Stamdata** (header data; content mandated §2.1, header position
   konvention): which patient; where and when treated or admitted; when
   treatment ended or discharge happened; "Eventuel cave skal anføres"; who it
   is sent to; sending date; the doctor responsible for the content; a contact
   number of the unit "så modtagende læge kan henvende sig i tvivlstilfælde".
2. **Anbefaling om opfølgning hos egen læge** (mandated first, §2.2): "en
   tydelig beskrivelse af, hvilken opfølgning der anbefales hos egen læge, og
   hvornår den bør foregå", each with a date or interval. Also any medical decision against
   resuscitation or to limit life-prolonging treatment, and any patient refusal
   of such treatment that is current, same illness, maintained at discharge.
   First line: the follow-up marking (section 8).
3. **Resumé af behandlingsforløb** (mandated §2.3), lettered: a) reason for
   admission or ambulatory course and referral diagnoses; b) relevant
   diagnoses, significant treatments and investigations, significant
   considerations and findings; c) important paraclinical results the GP must
   note (imaging, lab, pathology); d) coercive treatment under the psychiatric
   or somatic coercion acts, if relevant. Omit d) when not applicable.
4. **Patientinformation og -aftale** (mandated §2.4): what the patient and any
   relatives were told, what was agreed; for substitute consent, who consented
   and what they were told.
5. **Medicinoplysninger** (mandated §2.5): a) indication for every new
   prescription; b) reason for every change ("fx pausering af AK-behandling");
   c) when new or changed treatment stops, starts or changes; d) need for help
   with dispensing or administration; e) changes to dosisdispensering; f)
   medicine handed out, type and quantity. Write "Ingen ændringer" if none.
6. **Forebyggelses- og sundhedsfremmende plan** ("hvor det er relevant", §2.6):
   a) functional level; b) proposed sick leave and duration; c) social measures
   started (home care, social services); d) potential late effects or relapse
   symptoms; e) risk factors (smoking, alcohol, malnutrition, inactivity).
   Keep the heading; write "Ikke relevant" if nothing applies.
7. **Ikke-afsluttede og planlagte undersøgelser samt henvisninger** (mandated
   §2.7): results not yet available and that they will be forwarded; who tells
   the patient the result (default: the ordering clinician); investigations
   planned at the hospital; referrals elsewhere.
8. **Medicinliste** (mandated last, §2.8): the updated list "i overskuelig
   form" (table), "identisk med medicinoplysninger i FMK" and matching the list
   given to the patient. Per drug (§6): name, indication, form, strength, dose,
   frequency, route if relevant, stop date if any. Flag ny / ændret / uændret /
   seponeret (konvention).

## 3. Ambulatory-contact variant (§2)

For "andre typer af afslutning, fx fra ambulant behandling, lægevagt,
akutmodtagelser og præhospitale enheder" the epikrise "skal altid indeholde
oplysninger som anført i afsnittene 2.1-2.4 samt øvrige relevante oplysninger,
fx medicinændringer". So sections 1 to 4 always; 5, 7 and 8 whenever medicine
changed or anything is pending; 6 only where relevant; same headings and order
(konvention). Marking limited to Grøn or Hvid (DR). Long ambulatory courses:
send an interim epikrise "til orientering" during the course (§5).

## 4. Style rules (§2)

- "kortfattet og målrettet til patientens alment praktiserende læge": short,
  GP-oriented, no day-by-day narrative.
- "alment, forståeligt sprog"; no "specialespecifikke forkortelser, som
  modtageren ... ikke med rimelighed kan forventes at have kendskab til". Write
  specialty terms out; see terminology.md.
- Copied or auto-generated text "må kun indsættes, hvis det er relevant for
  egen læge": no pasted ward notes or raw lab dumps.
- Danish headings always; body language per task (v1: English body).

## 5. Coding, units, dates

- Diagnoses in words plus SKS code, aktionsdiagnose first, then bidiagnoser,
  e.g. "DI500 Kongestiv hjerteinsufficiens"; procedures as SKS codes with date
  (MedCom "Den gode epikrise" 2000: "officielle SKS-diagnoser"; konvention, not
  required by VEJ 10036; current MedCom XML standard UNVERIFIED).
- Drugs by substance name; brand in parentheses only if dispensed as such. ATC
  optional (UNVERIFIED as a requirement).
- Dates DD.MM.YYYY, times "kl. HH.MM" (MedCom example; konvention).
- Units: Danish SI lab convention, mmol/L, µmol/L, g/L, ×10⁹/L,
  mL/min/1,73 m² (UNVERIFIED: no primary unit source read).
- Patient identified by name and CPR-nummer (konvention).

## 6. Forbidden content and wording

- "foreløbig epikrise", "ikke-korrekturlæst epikrise" "eller lignende" (§2):
  no preliminary, draft, not proofread, awaiting review labels.
- Orders to the GP ("skal", "bedes"); use "anbefales" (§2.2).
- Specialty abbreviations without the written-out form (§2).
- Copied journal text irrelevant to the GP (§2).
- A Medicinliste that differs from FMK or the patient's list (§2.8).
- Headings from other national formats (Kern, Beleid, Entlassbrief) or
  English-only headings.
- Real patient data.

## 7. Header metadata (Stamdata fields, §2.1 and §5)

Patient (name, CPR); hospital and department; admission and discharge dates, or
contact date; cave; recipient GP practice; copy recipient if any; sending date;
responsible doctor (name, title); contact number; a line that a copy was given
to the patient or where it can be read electronically (§5 recommends either).
No status label of any kind (§2).

## 8. Follow-up marking: Rød, Gul, Grøn, Hvid

§3: the responsible doctor "skal tydeligt markere, om der er behov for
opfølgning hos egen læge". DR: every epikrise states whether follow-up is needed
(at minimum Grøn/Hvid); "Rød- og gulmarkering må kun anvendes efter indlæggelse
dvs. ikke i ambulante epikriser".

- **Rød**: follow-up "inden for 1-2 hverdage"; "helt ekstraordinært" (e.g.
  terminal patient without a palliative team); hospital also phones the GP.
- **Gul**: patient "særligt sårbar", not expected to contact the GP alone,
  needing active follow-up "inden for 14 hverdage" (table: 14 kalenderdage;
  write "14 dage"). E.g. clinically important adjustment or control of blood
  tests or medicine (anticoagulation, antipsychotics in dementia, opioids).
- **Grøn**: other epikriser with recommendations; patient contacts the GP.
- **Hvid**: no follow-up recommendation; information only.

DR notes the new MedCom standard derives the colour in the GP system from the
author's answers. In this experiment write it as the first line of section 2:
"Markering: Gul – opfølgning hos egen læge inden for 14 dage" (konvention).

## 9. Timing and copy (§5, §9)

Send "hurtigst muligt og inden for rimelig tid", never so late that the
recommended follow-up cannot start; no fixed day count (regional 3-hverdage
targets UNVERIFIED). Weekend or holiday discharge: inform home care etc.
independently of the epikrise. Patient copy, or where to read it electronically,
is recommended. The epikrise is part of the record.

## 10. Self-check

Run every item in [checklist.md](checklist.md) and fix failures. Often missed:
marking line; follow-up first; Medicinliste last and consistent with
Medicinoplysninger; indication per new drug; contact number; no "foreløbig".

## Sources

- VEJ nr 10036 af 30/11/2018: https://www.retsinformation.dk/eli/retsinfo/2018/10036 (PDF https://www.retsinformation.dk/api/pdf/204972)
- Danske Regioner 2019: https://www.regioner.dk/media/11371/faglig-vejledning-om-styrket-opfoelgning.pdf
- MedCom, Guide til den gode epikrise (2000): https://medcom.dk/wp-content/uploads/2023/03/guide-til-den-gode-epikrise.pdf
