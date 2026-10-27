# Template: Entlassbrief / Arztbrief (Germany)

Headings in conventional order (HL7 DE Entlassmanagementbrief / Arztbrief Plus); the numbered § 9 Abs. 3 items are tagged [§9-n]. Replace every <placeholder>; write "keine" / "entfällt" rather than deleting a heading.

---

<Klinikname>, <Fachabteilung>, <Anschrift>
<Ort>, <DD.MM.JJJJ>

**<Vorläufiger | Endgültiger> Entlassbrief** [§9-3]
Rule: exactly one label, in the title.

An: <Hausarzt/-ärztin Name, Praxisanschrift>
Rule: addressee is the weiterbehandelnder Arzt; copies (einweisender Arzt, Reha) listed separately.

**Patient/in:** <Nachname, Vorname>, geb. <DD.MM.JJJJ>, <Anschrift>, Versichertennr. <…> [§9-1]
**Aufnahme:** <DD.MM.JJJJ> **Entlassung:** <DD.MM.JJJJ> [§9-1]
**Behandelnde/r Arzt/Ärztin:** <Name, Funktion> **Telefon für Rückfragen:** <Nummer> [§9-2]
Rule: the number is for the Hausarzt; § 3 Abs. 7 requires an Ansprechpartner Mo–Fr 09:00–19:00, Sa/So 10:00–14:00.

## Anrede (salutation)
Sehr geehrte Frau Kollegin <Name>, sehr geehrter Herr Kollege <Name>,
wir berichten über <Herrn/Frau Vorname Nachname>, geb. <DD.MM.JJJJ>, <der/die> sich vom <DD.MM.JJJJ> bis <DD.MM.JJJJ> in unserer stationären Behandlung befand.
Rule: Sie-form, colleague as reader, patient named once with Geburtsdatum.

## Grund der Einweisung (reason for admission) [§9-4]
<One or two sentences: who referred, presenting problem, route (Hausarzt / Rettungsdienst / Notaufnahme).>
Rule: reason at admission, not the final diagnosis.

## Diagnosen (diagnoses) [§9-5]
1. Hauptdiagnose: <Text> (<ICD-10-GM>)
2. Nebendiagnose: <Text> (<ICD-10-GM>)
3. <…>
Multiresistente Erreger: <kein Nachweis | Nachweis von …, Screening vom DD.MM.JJJJ>
Rule: Hauptdiagnose first, code after text, MRE line always present.

## Allergien/Unverträglichkeiten (allergies and intolerances)
<Substanz – Reaktion | keine bekannt>
Rule: drug intolerances required by § 9 item 9.

## Anamnese (history)
<Presenting complaint and course before admission; relevant Vorerkrankungen; Medikation bei Aufnahme with Stärke and Dosierschema; social situation if relevant to follow-up.>
Rule: prose; drugs on admission listed here so changes can be traced.

## Befunde (findings)
**Aufnahmebefund <DD.MM.JJJJ>:** <RR … mmHg, HF …/min, Temp …°C, SpO2 … %, key exam findings>
**Labor:** <parameter value unit (DD.MM.JJJJ) → value unit (DD.MM.JJJJ)>
**Bildgebung/Funktionsdiagnostik:** <modality DD.MM.JJJJ: result>
Rule: dates on every result, decimal comma, source units; trends not full tables.

## Entlassungsbefund (status at discharge) [§9-6]
<Clinical state, vitals at discharge, key discharge labs, Mobilität, Kognition, Wundstatus.>
Rule: present tense; this is the baseline the Hausarzt compares against.

## Epikrise (narrative course) [§9-7]
<Why the diagnosis was made (Anamnese + Diagnostik), what was done (Therapie, Prozeduren with OPS where known, dates), response, complications, open questions.>
Rule: title is exactly "Epikrise"; interpretation, not a repeat of Befunde.

## Weiteres Prozedere/Empfehlungen (further plan) [§9-8]
- Wir bitten um <Kontrolle/Maßnahme> am/bis <DD.MM.JJJJ>.
- Ausstehende Befunde: <…> | keine. <If vorläufig: "Ein endgültiger Entlassbrief folgt nach Eingang von …">
- Wiedervorstellung: <wann, wo> | nicht vorgesehen.
Rule: each line concrete, dated, addressed to the Hausarzt.

## Medikation bei Entlassung (medication at discharge) [§9-9]
- <Wirkstoff> <Stärke> <Darreichungsform>, <Mo-Mi-Ab-zN>, <Therapiedauer: Dauermedikation | bis DD.MM.JJJJ> — <neu | geändert | unverändert | abgesetzt>: <Begründung>
- <…>
Abgesetzt: <Wirkstoff> — <Begründung> | keine.
Rule: INN naming, four-part Dosierschema, every change explained.

**Medikationsplan** (BMP-Spalten, V2.8)
| Wirkstoff | Handelsname | Stärke | Form | Mo | Mi | Ab | zN | Einheit | Hinweise | Grund |
|---|---|---|---|---|---|---|---|---|---|---|
| *Dauermedikation* | | | | | | | | | | |
| <…> | <…> | <…> | <Tabl.> | <1> | <0> | <1> | <0> | <Stück> | <…> | <…> |
| *zeitlich befristet anzuwendende Medikamente* | | | | | | | | | | |
| <…> | | | | | | | | | | |
| *Bedarfsmedikation* | | | | | | | | | | |
| <…> | | | | | | | | | | |
Rule: four filled dose positions or Freitext ("bei Bedarf") across the dose columns; decimal comma; Zwischenüberschriften from the BMP list.

**Mitgegebene Arzneimittel:** <Wirkstoff, Menge, bis einschließlich DD.MM.JJJJ> | keine
Rule: required even when none.

## Veranlasste Leistungen und Arbeitsunfähigkeit (ordered services, sick-note) [§9-10]
- Verordnungen: <Heil-/Hilfsmittel, häusliche Krankenpflege, SAPV, DiGA, Reha-Antrag> | keine
- Arbeitsunfähigkeit: <AU-Bescheinigung ausgestellt bis DD.MM.JJJJ> | entfällt (<Begründung, z. B. Rentner/in>)
Rule: both lines always present.

## Nachfolgende Versorgungseinrichtung (next care setting) [§9-11]
<häusliches Umfeld, hausärztliche Weiterbehandlung | Reha-Klinik Name ab DD.MM.JJJJ | Pflegeeinrichtung Name>
Rule: name the setting; add Pflegedienst if involved.

## Mitgegebene Befunde (results handed to the patient) [§9-12]
<Liste: Röntgen-Thorax Befund DD.MM.JJJJ, Laborausdruck, Medikationsplan, …> | keine
Rule: list what the patient physically carries.

## Abschließende Bemerkungen (closing)
Für Rückfragen stehen wir Ihnen unter <Telefonnummer> gern zur Verfügung.

Mit freundlichen kollegialen Grüßen

<Name, Oberarzt/-ärztin oder Chefarzt/-ärztin>    <Name, Stationsarzt/-ärztin>
Rule: Grußformel and two signatures close the letter.
