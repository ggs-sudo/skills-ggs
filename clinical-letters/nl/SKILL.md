---
name: nl-ontslagbericht-hasp
description: Write the ontslagbericht, the Dutch specialist's discharge message to the huisarts (GP), for a patient treated in a Dutch hospital in the Netherlands, in the fixed Envelop / Kern / Dossiersamenvatting structure of the NHG-FMS Richtlijn HASP. Use for any letter to the GP in the Netherlands, kliniek or polikliniek. Read template.md for heading order and checklist.md before finishing.
---

# nl-ontslagbericht-hasp: letter to the GP in the Netherlands

Source of every rule: NHG and Federatie Medisch Specialisten, "Richtlijn
Informatie-uitwisseling tussen huisarts en medisch specialist (Richtlijn HASP)",
3rd ed., Dec 2017, cited by chapter (H), appendix (B) and summary card (SK).
The Oct 2024 reprint is textually identical except one AGB-code note (see 9).
(konventie) = Dutch practice, not in HASP; (UNVERIFIED) = no source read.

Workflow: 1) read this file; 2) build on [template.md](template.md); 3) check
terms in [terminology.md](terminology.md); 4) compare register with
[example.md](example.md); 5) run [checklist.md](checklist.md) before finishing.

## 1. Scope and addressee

- HASP message types: verwijsbericht, update, ontslagbericht (H2.2); the
  ontslagbericht replaced the "ontslagbrief" (H1.2). Sent at discharge from
  poliklinische controle, discharge home, transfer to another institution or
  ward (H2.2, B-A).
- Addressee: at discharge home, the huisarts. At discharge to another
  institution (verpleeghuis, revalidatie) that institution is addressee and the
  huisarts "krijgt verplicht een kopie" (H7.3, SK). One primary addressee.
- The Kern must show the GP "snel ... wat het antwoord van de medisch
  specialist is op de vraagstelling, en welke follow-up de huisarts moet
  bieden" (H3.3). Order is reversed from hospital habit: "eerst de
  eindconclusie en gewenste nazorg ... in de Kern, en dan pas de
  onderbouwing, in de Dossiersamenvatting" (H5.1).

## 2. Three-part structure

"Alle berichten hebben een vaste indeling in drie delen: Envelop, Kern en
Dossiersamenvatting" (H3.1), in that order. Envelop = logistics and contact
data; Kern = "compact de relevantste informatie voor de continuïteit van
zorg"; Dossiersamenvatting = record extracts, read "screenend" by the GP for
new medication and results (H5.1).

Asterisks (H5): `*` verplicht in ontslagbericht; `**` in update; `***` bij
kwetsbare ouderen. "Verplichte rubrieken worden altijd gepresenteerd bij de
ontvanger, ook als ze niet zijn ingevuld"; an empty mandatory rubriek gets the
text "geen" (H7.3). Use rubriek names exactly as HASP spells them; never add,
rename or drop rubrieken ("extra rubrieken worden niet ondersteund door de
HIS'en", H7.5). Optional rubrieken may be omitted.

## 3. Required rubrieken in order

### Envelop (H5.1, Tabel 7.1)
Gegevens auteur* (institution, responsible specialist, contactpersoon with
"wanneer en hoe deze bereikt kan worden"); Gegevens patiënt of cliënt* (BSN,
name, sex, date of birth, address, contactpersoon if relevant); Gegevens
geadresseerde*; Gegevens kopie-ontvanger(s); Datum en tijd* (moment of
authorisation); Type bericht* (one of "update polikliniek, ontslagbericht
polikliniek, update kliniek, ontslagbericht kliniek"); Zorgpad and Urgentie
(only with regional agreements); Beheerder bericht* (archiving organisation,
usually the sender). Identifiers URA, UZI, AGB when known.

### Kern (H5.1, Tabel 7.2) - this exact order
1. Reden bericht* (reason): "Maak duidelijk ... hoelang, waarvoor en via welke
   route (verwijzing, spoedeisende hulp, anders) de patiënt opgenomen is
   geweest en waar patiënt nu naartoe gaat." Outpatient: "Ontslag uit
   poliklinische controle. Laatste bezoek was <date>. U verwees ... in verband
   met ...". Admission via SEH must be stated here (B.2).
2. Conclusie, diagnose* (conclusion, diagnosis): "kernachtige samenvatting van
   conclusie of diagnose, inclusief uw eigen overwegingen op dit moment";
   diagnosis or working hypothesis, response to treatment, prognosis if known,
   diagnosis made elsewhere named as such; "Bedenk of de verwijsvraag is
   beantwoord." "NB hier geen nader verklarende details, die komen ... in de
   Dossiersamenvatting." Frail elderly: state whether a delier occurred (B.3).
3. Beleid* (management): "beleid en behandeling die nu actueel zijn geworden.
   Bij medicatiewijziging: wat is precies gewijzigd, welk middel gestaakt of
   verlaagd, welk gestart of verhoogd. Welke diagnostiek is aangevraagd en nog
   open staat. NB hier niet het voorschrift vermelden, dat komt in de
   Dossiersamenvatting." Deviations from the default division of
   responsibility go here and/or in Aanbeveling uw follow-up (H2.4).
4. Aanbeveling uw follow-up* (recommended follow-up by you): "de ... gevraagde
   nazorg door degene aan wie het bericht is gericht ... Ook de controles die
   deze moet uitvoeren en wat die controles inhouden; ook al of niet
   voortzetten medicatie. Eventueel advies voor doorverwijzing." After an
   admission include advice from consulted specialties (SK).
5. Afgesproken met patiënt (agreed with patient; optional): "De
   verantwoordelijkheid die met de patiënt is afgesproken", e.g. patient books
   the GP visit, or may contact the ward directly until a stated date.
6. Verder van belang (also of note; optional): a few words pointing to a
   Dossiersamenvatting rubriek the GP must not miss, e.g. "Zie Behandelgrenzen."

Beleid, Aanbeveling uw follow-up and Afgesproken met patiënt must agree:
"tezamen geven die de duidelijkheid ... over de onderlinge afspraken" (H7.3).

### Dossiersamenvatting (Tabel 7.3) - this order; optional unless marked
Voorgeschiedenis; Anamnese (mark heteroanamnese); Beloop, interventie;
Familieanamnese (disease plus relation); Psychosociale anamnese (restraint);
Risicovol leefgedrag* (alcohol, tobacco, drugs, sexual risk; "Ook negatieve
bevindingen" if asked); Lichamelijk onderzoek (positive and negative
findings); Laboratoriumonderzoek ("per onderzoek datum, plaats, type bepaling,
materiaal en waarde", units, reference values where relevant); Beeldvormend
onderzoek; Functieonderzoek (ECG, lung function); Psychogeriatrisch
onderzoek***; Overig aanvullend onderzoek; Intercollegiale consulten (consult
geriater always, SK); Verrichtingen derden; Medicatie* ("medicatieafspraken
voor zover bekend bij de verzender": the prescriptions, stopped drugs with
reason); Overgevoeligheid voor medicatie; contra-indicaties voor
voorschrijven* (detail enough to judge re-exposure, serious side effects);
Profylaxe* (precautions at procedures); Behandelgrenzen*** ("Precies ...
welke afspraak is gemaakt, met wie, en wanneer").

## 4. Kliniek vs polikliniek

- Kliniek: Type bericht "ontslagbericht kliniek"; Reden bericht gives dates of
  stay, route of admission, destination. Follow-up and patient agreements from
  an admission appear only in the ontslagbericht, never in a kliniek update
  (H5.2). Deadline: "in principe direct maar uiterlijk binnen 24 uur" (H2.3).
- Polikliniek: Type bericht "ontslagbericht polikliniek"; Reden bericht opens
  with "Ontslag uit poliklinische controle", last visit date, original
  referral reason. Deadline: "uiterlijk binnen 5 dagen" (H2.3).
- Pending results are sent later as an update, never a reason to delay:
  "tijdigheid ... prevaleert boven volledigheid" (H2.3, H5.1).
- Responsibility (H2.4): after kliniek discharge the complaint stays with the
  specialist unless stated otherwise, other care returns to the GP; after
  polikliniek discharge everything returns to the GP.

## 5. Style rules

- Dutch; GP addressed as "u"; first person, short declaratives as in the H5
  examples ("Ik zag patiënt ...", "Ik startte ..."). Beleid "beknopt en
  puntsgewijs" (SK); number problems and cross-refer with "Ad 1." (H5 ex. 4).
- Abbreviations: "Het gebruik van afkortingen ... leidt vaak tot verwarring en
  soms tot fouten ... en verdient daarom zeer terughoudend gebruik" (H3.3,
  H7.5). Write terms out; see terminology.md.
- Check system-filled rubrieken "op volledigheid, relevantie en privacy"
  (H7.3); patients read these messages, so avoid needless complexity (B-D.5).

## 6. Coding, units, dates

- HASP mandates no code system; rubrieken have "Relatie met ZIB: nog niet
  aangegeven" (Tabel 7.2-7.3). A code, if given, carries its description
  (H7.3). ICD-10, DBC, ICPC, ATC usage is (konventie), see terminology.md.
- HASP fixes no date notation; its examples vary (H3.1). Use one notation
  throughout; DD-MM-JJJJ is standard Dutch (konventie). Date every result and
  medication line, as every H5 example does.
- Units as in H5: mmol/l, µmol/l, mg/l, U/l, mmHg, kg, cm; decimal comma in
  Dutch text ("7,9").

## 7. Forbidden

- Prescription details (dose schedules) in Beleid; they go in Medicatie.
- Explanatory detail or decursus in Conclusie, diagnose.
- New, renamed or dropped rubrieken; an empty mandatory rubriek (write "geen").
- A follow-up request hidden in Beleid or the Dossiersamenvatting instead of
  Aanbeveling uw follow-up.
- Undated results or medication; unexplained abbreviations; invented data.

## 8. Deadlines and versions

Kliniek 24 h; polikliniek 5 days; later results by update. The Oct 2024
reprint adds one note under H1.3: the rule that the AGB-code must be the
personal code is dropped, "zowel de persoonlijke als de praktijkcode" may be
used. No rubriek, order, definition or deadline changed.

## 9. Self-check

Run [checklist.md](checklist.md); every item must be yes.

## Sources

- https://www.nhg.org/wp-content/uploads/2022/10/Richtlijn-Gegevensuitwisseling-Huisarts-en-Specialist-HASP.pdf
- https://www.nhg.org/wp-content/uploads/2022/11/Richtlijn-HASP-Samenvatting.pdf
- https://www.nhg.org/wp-content/uploads/2022/10/241212-Richtlijn-Informatie-uitwisseling-tussen-huisarts-en-medisch-specialist_2018_v_okt2024_Web-up.pdf
