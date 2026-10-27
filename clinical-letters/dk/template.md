# Epikrise template (VEJ 10036 order)

Fill every `<placeholder>`. Keep headings verbatim in Danish; the English in
parentheses may be kept or dropped. Order is fixed: Stamdata header, then
Anbefaling first (§2.2), Medicinliste last (§2.8); sections 3 to 7 follow the
vejledning numbering. Ambulatory contact: sections 1 to 4 always, 5/7/8 when
medicine changed or anything is pending, 6 when relevant; marking Grøn/Hvid only.

---

# Epikrise

## Stamdata (Header data)
Patient: <full name>, CPR-nr.: <DDMMYY-XXXX>
Behandlingssted: <hospital>, <department>, <ward or clinic>
Indlagt: <DD.MM.YYYY>   Udskrevet: <DD.MM.YYYY>   (ambulant: Kontaktdato: <DD.MM.YYYY>)
Cave: <allergies and intolerances, or "Ingen kendte">
Modtager: <GP practice name and address> (egen læge)
Kopi til: <referring speciallæge or vagtlæge, or omit the line>
Afsendt: <DD.MM.YYYY>
Ansvarlig læge: <name>, <title>
Kontaktnummer: <department phone, hours>
Kopi til patienten: <"udleveret" or "kan læses på sundhed.dk">
Rule: all §2.1 items present; no status word such as foreløbig or draft.

## Anbefaling om opfølgning hos egen læge (Recommended follow-up with own GP)
Markering: <Rød | Gul | Grøn | Hvid> – <one-clause reason and deadline>
- <what is recommended>, <by when or interval>
- <next item>
Genoplivning/behandlingsniveau: <decision or "Ingen beslutning truffet">
Rule: first substantive section; each item has an action and a time; wording is
"anbefales", not orders; Rød/Gul only after admission.

## Resumé af behandlingsforløb (Summary of the course)
a) Årsag til indlæggelse og henvisningsdiagnoser: <reason>; <referral diagnosis>
b) Diagnoser, behandling, undersøgelser og fund:
   Aktionsdiagnose: <SKS code> <name in words>
   Bidiagnoser: <SKS code> <name>; <...>
   <2 to 6 sentences: key treatments, investigations, considerations>
c) Vigtige parakliniske resultater: <imaging / lab with values and units / pathology>
d) Tvang: <only if used and relevant; otherwise omit the line>
Rule: concise, GP-relevant, no copied journal text, no unexplained abbreviations.

## Patientinformation og -aftale (Information given and agreed with the patient)
<what the patient and relatives were told; what was agreed; who consented if
substitute consent>
Rule: concrete content, not "informed about condition".

## Medicinoplysninger (Medication information)
Nyt: <drug> – indikation: <...>; <start date>; <planned duration or review>
Ændret: <drug> – <old → new dose>; begrundelse: <...>; <when to review or stop>
Pauseret/seponeret: <drug> – begrundelse: <...>; genoptages <date or condition>
Dispensering/administration: <help needed, or "Ingen behov">
Dosisdispensering: <change communicated to pharmacy, or "Uændret">
Medgivet medicin: <type and quantity, or "Ingen">
Rule: every new drug has an indication; every change has a reason and a date;
write "Ingen ændringer" if nothing changed.

## Forebyggelses- og sundhedsfremmende plan (Prevention and health promotion plan)
Funktionsniveau: <...>
Sygemelding: <proposal and expected duration, or "Ikke relevant">
Socialmedicinske foranstaltninger: <home care, municipality, or "Ingen">
Senfølger/recidiv: <symptoms the GP should watch for>
Risikofaktorer: <smoking, alcohol, nutrition, inactivity>
Rule: keep the heading; write "Ikke relevant" where nothing applies.

## Ikke-afsluttede og planlagte undersøgelser samt henvisninger (Pending and planned investigations, referrals)
Afventer svar: <test>, eftersendes; patienten informeres af <ordering clinician or unit>
Planlagt på sygehuset: <appointment or test, date>
Henvist til: <other unit or service, date>
Rule: say who tells the patient each pending result; "Ingen" if nothing pending.

## Medicinliste (Medication list)
| Lægemiddel (generisk navn) | Indikation | Form | Styrke | Dosis og hyppighed | Adm.vej | Ophør | Status |
|---|---|---|---|---|---|---|---|
| <name> | <indication> | <tablet etc.> | <strength> | <dose x times/day> | <oral etc.> | <date or –> | <ny / ændret / uændret / seponeret> |
Ajourført i FMK: <DD.MM.YYYY>. Listen er identisk med den medicinliste, patienten har fået.
Rule: last section; identical to FMK and to the patient's list; one row per drug.
