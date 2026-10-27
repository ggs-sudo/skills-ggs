---
name: de-arztbrief
description: Write a German hospital physician letter (Arztbrief / Entlassbrief) to the Hausarzt in the structure required by the Rahmenvertrag Entlassmanagement § 9 and HL7 DE Arztbrief Plus. Use for Germany, a German hospital, a Hausarzt, an Arztbrief, an Entlassbrief, or a "letter to the GP in Germany". Read template.md for heading order and checklist.md before finishing.
---

# de-arztbrief: Entlassbrief / Arztbrief to the Hausarzt

## Scope and addressee
- Document: physician-authored Entlassbrief closing a hospital episode; the same structure serves an ambulatory Arztbrief to the referring doctor.
- Addressee: the weiterbehandelnder Arzt, normally the Hausarzt. The patient receives the letter on the day of discharge and carries it (§ 3 Abs. 7, § 9 Abs. 1). With consent the einweisender Arzt and a receiving Reha/Pflege institution also get it.
- Legal basis: Rahmenvertrag Entlassmanagement nach § 39 Abs. 1a SGB V, Lesefassung 14. Änderungsvereinbarung vom 19.11.2025, in force 01.04.2026; § 9 is unchanged from the 13. ÄndVb (23.05.2025). "Der Entlassbrief ist zwingender Bestandteil des Entlassmanagements" (§ 9 Abs. 1).
- Binding = the 12 minimum items. Conventional = heading order, heading wording, register (HL7 DE Arztbrief Plus / Entlassmanagementbrief and German practice).

## The 12 binding minimum items (§ 9 Abs. 3: "Diese sind mindestens:")
Each must appear, even as "keine" / "entfällt".
1. Patientenstammdaten, Aufnahme- und Entlassdatum.
2. Name des behandelnden Krankenhausarztes und Telefonnummer für Rückfragen.
3. Kennzeichnung „vorläufiger“ oder „endgültiger“ Entlassbrief.
4. Grund der Einweisung (reason for admission).
5. Diagnosen (Haupt- und Nebendiagnosen) einschließlich Infektionen oder Besiedelungen durch multiresistente Erreger (state MRE even when negative).
6. Entlassungsbefund (status at discharge).
7. Epikrise (Anamnese, Diagnostik, Therapien inkl. Prozeduren).
8. Weiteres Prozedere/Empfehlungen.
9. Arzneimittel "unter ihrer Wirkstoffbezeichnung/-stärke ...; Darreichungsform ...; Dosierung bei Aufnahme/Entlassung mit Therapiedauer, Erläuterung bei Veränderungen, bekannte Arzneimittelunverträglichkeiten" und der Medikationsplan; Information über mitgegebene Arzneimittel.
10. Alle veranlassten Leistungen (Heil-/Hilfsmittel, häusliche Krankenpflege, SAPV, DiGA, Reha) und Information über Bescheinigung der Arbeitsunfähigkeit.
11. Nachfolgende Versorgungseinrichtung.
12. Mitgegebene Befunde.

## Conventional section order (German heading, gloss, rule)
From the HL7 DE Entlassmanagementbrief v1.1 section table and Arztbrief Plus body; not mandated by § 9. Use headings verbatim; skeleton in [template.md](template.md).
1. Briefkopf: Klinik, Abteilung, Patientenstammdaten, Aufnahme-/Entlassdatum, title with vorläufig/endgültig, behandelnder Arzt, Telefonnummer. Items 1–3.
2. Anrede: "Sehr geehrte Frau Kollegin, sehr geehrter Herr Kollege," then one sentence naming the patient with Geburtsdatum and the stay dates (Arztbrief Plus § 6.7 form).
3. Grund der Einweisung: one or two sentences. Item 4.
4. Diagnosen: numbered, Hauptdiagnose first, then Nebendiagnosen, each with ICD-10-GM code; last line multiresistente Erreger (positive or "kein Nachweis"). Item 5.
5. Allergien/Unverträglichkeiten: list or "keine bekannt". Covers the Arzneimittelunverträglichkeiten of item 9.
6. Anamnese: presenting complaint, relevant Vorerkrankungen, Medikation bei Aufnahme with doses, social context relevant to follow-up.
7. Befunde: Aufnahmebefund, Labor, Bildgebung, Funktionsdiagnostik with dates and values; trends, not every value.
8. Entlassungsbefund: clinical state, vitals, key discharge labs, Mobilität. Item 6.
9. Epikrise (title must be exactly "Epikrise", Arztbrief Plus § 6.21): interpretation of the course for the colleague — why diagnosed, what was done (Prozeduren, OPS where known), response, open questions. Item 7.
10. Weiteres Prozedere/Empfehlungen: concrete, dated requests to the Hausarzt ("Wir bitten um ..."), ausstehende Befunde, and when the endgültiger Brief follows if vorläufig. Item 8.
11. Medikation bei Entlassung: one line per drug (rules below) with every change explained, then the Medikationsplan table, then "Mitgegebene Arzneimittel". Item 9.
12. Veranlasste Leistungen und Arbeitsunfähigkeit: each Verordnung or "keine"; "AU-Bescheinigung ausgestellt bis DD.MM.JJJJ" or "entfällt (Begründung)". Item 10.
13. Nachfolgende Versorgungseinrichtung: häusliches Umfeld / Reha / Pflegeeinrichtung, name and date. Item 11.
14. Mitgegebene Befunde: list. Item 12.
15. Abschließende Bemerkungen: "Für Rückfragen stehen wir Ihnen unter ... gern zur Verfügung." Grußformel "Mit freundlichen kollegialen Grüßen", signatures (Oberarzt/Chefarzt, Stationsarzt).

## vorläufig / endgültig
- Label in the document title: "Vorläufiger Entlassbrief" or "Endgültiger Entlassbrief" (§ 9 Abs. 3; HL7 DE: "Der Titel sollte bei einem vorläufigen Entlassbrief das Wort vorläufig enthalten"). Exactly one label, never none.
- A vorläufiger Brief is issued when the final one is not possible at discharge and must still contain "alle getroffenen Maßnahmen und Verordnungen" (§ 9 Abs. 2); name what is outstanding and that the endgültiger Entlassbrief follows.

## Medication and Medikationsplan
- Name drugs by Wirkstoff (INN, German spelling); Handelsname optional in parentheses. § 115c SGB V: prefer substances available in ambulatory care.
- Per line: Wirkstoff Stärke Darreichungsform, Dosierschema, Therapiedauer, status (neu / geändert / unverändert / abgesetzt) and Begründung for every change.
- Dosierschema in the four-part notation morgens-mittags-abends-zur Nacht (1-0-1-0) with all four positions filled, or Freitext such as "bei Bedarf"; decimal comma, "0,5" not ",5"; fractions ½ ¼ ¾ allowed (BMP V2.8, A 2.6–A 2.7).
- Medikationsplan is required from three prescribed drugs (§ 7 Abs. 3); include the table anyway. BMP column order (Tabelle 1): Wirkstoff | Handelsname | Stärke | Form | Mo | Mi | Ab | zN | Einheit | Hinweise | Grund. Group rows under BMP Zwischenüberschriften: Dauermedikation, Bedarfsmedikation, zeitlich befristet anzuwendende Medikamente, Selbstmedikation.
- The Medikationsplan "ersetzt nicht" the information to the weiterbehandelnder Arzt (§ 7 Abs. 3): keep the narrative lines too.
- Mitgegebene Arzneimittel: name, amount, reach ("bis einschließlich DD.MM.JJJJ") or "keine".

## Style
- Formal letter, Sie-form, written to the colleague, never to the patient. Anamnese, Epikrise, Prozedere are prose; Diagnosen, Befunde, Medikation may be lists.
- Anrede and Grußformel are part of the convention (Arztbrief Plus sections Anrede, Abschließende Bemerkungen).
- Past tense for the course, present tense for discharge status, polite requests ("Wir bitten um Kontrolle des Kreatinins am ...").
- Z.n., V.a., o.B., DD, i.v., p.o. are usual in German letters; use sparingly, never for a Hauptdiagnose. See [terminology.md](terminology.md).
- v1 convention: body may be English with German headings; headings, labels, Anrede and Grußformel stay German.

## Coding, units, dates
- ICD-10-GM for diagnoses, code after the text ("Pneumonie, nicht näher bezeichnet (J18.9)"); OPS for procedures; ATC/PZN only if the record supplies them (Arztbrief Plus uses ICD-10 GM, OPS, WHO ATC, PZN).
- Dates DD.MM.JJJJ, times HH:MM Uhr. Decimal comma (CRP 184,3 mg/l; 38,6 °C). Keep source units (mmol/l, mg/dl, g/dl, /µl); "RR 135/80 mmHg", "HF 88/min", kg, cm.

## Forbidden
- Missing label, missing Telefonnummer, addressee other than the treating colleague.
- Brand-only drug names; a dose without Stärke, Form and Dosierschema; a change without Begründung.
- Omitting any of the 12 items (write "keine"/"entfällt").
- Foreign headings ("Hospital course", "Kern", "Discharge summary"), US dates, decimal point.
- Speculation stated as diagnosis: use "V.a." or "DD" plus a plan to resolve it.
- Real patient identifiers; patient-facing instructions inside the physician letter.

## Header metadata
- Klinik, Fachabteilung, address, letter date. Patient: Name, Vorname, Geburtsdatum, Anschrift, Krankenversichertennummer if available. Aufnahmedatum, Entlassdatum (DD.MM.JJJJ).
- Behandelnder Arzt (name, function) and "Telefon für Rückfragen" with the number; § 3 Abs. 7 requires an Ansprechpartner reachable Mo–Fr 09:00–19:00, Sa/So 10:00–14:00 (state the number, not the hours).

## Self-check
Read [checklist.md](checklist.md) before finishing and fix every failed item; compare form with [example.md](example.md).

## Sources (read directly)
- Rahmenvertrag Entlassmanagement, Lesefassung 14. ÄndVb 19.11.2025 (in force 01.04.2026), § 3 Abs. 7–8, § 7 Abs. 3, § 9: https://www.dkgev.de/fileadmin/Mediapool/2_Themen/2.3_Versorgung-Struktur/2.3.3_Entlassmanagement/Lesefassung_des_Rahmenvertrages_Entlassmanagement_i.d.F._der_14._AEnderungsvereinbarung_vom_01.04.2026.pdf (13. ÄndVb 23.05.2025 checked: § 9 identical).
- HL7 DE IG Entlassmanagementbrief v1.1 (04.12.2020): https://wiki.hl7.de/index.php?title=IG:Entlassmanagementbrief
- HL7 DE IG Arztbrief Plus (wiki v3.15 24.08.2020; PDF v3.12): https://wiki.hl7.de/index.php?title=IG:Arztbrief_Plus ; https://download.hl7.de/documents/cdar2-arztbrief/ArztbriefPlus-v312.pdf
- KBV/BÄK/DAV BMP-Spezifikation V2.8 (01.10.2025): https://www.kbv.de/documents/infothek/rechtsquellen/weitere-vertraege/praxen/medikationsplan/medikationsplan-anlage-3.pdf
- KBV MIO Krankenhaus-Entlassbrief 1.0.0 (background page only; content model UNVERIFIED): https://hub.kbv.de/spaces/KHE1X0X0/pages/88998214/Hintergrundinformationen
