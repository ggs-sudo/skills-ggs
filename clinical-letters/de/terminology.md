# Terminology: EN → German for the Entlassbrief

## Section headings (use verbatim)
| English | German heading | Note |
|---|---|---|
| Letterhead / header | Briefkopf | Klinik, Patient, Daten, Arzt, Telefon |
| Provisional / final discharge letter | Vorläufiger / Endgültiger Entlassbrief | label in title (§ 9 Abs. 3) |
| Salutation | Anrede | Arztbrief Plus section 1.2.276.0.76.10.3001 |
| Reason for admission / referral | Grund der Einweisung (Rahmenvertrag) / Grund der Überweisung (Arztbrief Plus) | use "Grund der Einweisung" for inpatients |
| Diagnoses, main / secondary | Diagnosen, Hauptdiagnose / Nebendiagnosen | ICD-10-GM |
| Admission / discharge diagnosis | Aufnahmediagnose / Entlassungsdiagnose | Arztbrief Plus sections |
| Multiresistant organisms | Multiresistente Erreger (MRE), Infektionen oder Besiedelungen | always one line |
| Allergies, intolerances, risks | Allergien, Unverträglichkeiten, Risiken | |
| History (present / past / family / social) | Anamnese (Jetzige Anamnese / Frühere Erkrankungen / Familienanamnese / Sozialanamnese) | |
| Findings, results | Befunde / Erhobene Befunde / Befunde/Ergebnisse | |
| Findings at discharge | Entlassungsbefund | Rahmenvertrag term; HL7 DE "Entlassungsbefunde" |
| Hospital course / narrative summary | Epikrise (Zusammenfassung des Aufenthalts) | title must be "Epikrise" |
| Procedures | Prozeduren und Maßnahmen | OPS |
| Further plan / recommendations | Weiteres Prozedere/Empfehlungen (Weitere empfohlene Maßnahmen) | |
| Medication on admission / during stay / at discharge | Medikation bei Einweisung (Aufnahme) / während des Aufenthalts / bei Entlassung | |
| Medication plan | Medikationsplan (bundeseinheitlicher Medikationsplan, BMP) | § 31a SGB V |
| Medicines handed over | Mitgegebene Arzneimittel | |
| Ordered services / prescriptions | Veranlasste Leistungen / Verordnungen | Heil-/Hilfsmittel, häusliche Krankenpflege, SAPV, DiGA |
| Sick-note / certificate of incapacity for work | Arbeitsunfähigkeitsbescheinigung (AU-Bescheinigung) | "entfällt" with reason if none |
| Next care setting | Nachfolgende Versorgungseinrichtung | häusliches Umfeld, Reha, Pflegeeinrichtung |
| Results handed to the patient | Mitgegebene Befunde | |
| Attachments | Beilagen/Anhang | |
| Closing remarks | Abschließende Bemerkungen | contains Grußformel |

## Letter phrases
| English | German |
|---|---|
| Dear colleague (f / m) | Sehr geehrte Frau Kollegin, / Sehr geehrter Herr Kollege, |
| We report on Mr/Ms X, born …, who was under our inpatient care from … to … | wir berichten über Herrn/Frau X, geb. …, der/die sich vom … bis … in unserer stationären Behandlung befand |
| Thank you for referring | Vielen Dank für die freundliche Überweisung / Einweisung |
| We ask you to … | Wir bitten um … |
| We recommend … | Wir empfehlen … |
| Please re-refer if … | Wir bitten um Wiedervorstellung bei … |
| Outstanding results | Ausstehende Befunde |
| A final discharge letter will follow | Ein endgültiger Entlassbrief folgt |
| We are glad to answer questions on … | Für Rückfragen stehen wir Ihnen unter … gern zur Verfügung |
| With kind collegial regards | Mit freundlichen kollegialen Grüßen (Arztbrief Plus example: "mit kollegialen Grüßen") |
| Treating physician / senior physician / head physician | Stationsarzt/-ärztin / Oberarzt/-ärztin / Chefarzt/-ärztin |
| General practitioner | Hausarzt/Hausärztin (weiterbehandelnder Arzt) |
| Referring physician | einweisender Arzt |
| none / not applicable / none known | keine / entfällt / keine bekannt |
| new / changed / unchanged / stopped | neu / geändert / unverändert / abgesetzt |
| long-term / as needed / time-limited | Dauermedikation / Bedarfsmedikation / zeitlich befristet (BMP Zwischenüberschriften) |

## Code systems
| Use | System | Form |
|---|---|---|
| Diagnoses | ICD-10-GM (German Modification, annual version; BfArM) | "Text (J18.9)"; use the terminal code with ".x" digits as in ICD-10-GM, e.g. I10.00, E11.90 |
| Procedures | OPS (Operationen- und Prozedurenschlüssel, BfArM) | "Text (OPS 1-632)" where known |
| Drug substance | Wirkstoffbezeichnung (INN, German spelling); ATC optional | "Ramipril 5 mg Tabl." |
| Drug product | PZN (Pharmazentralnummer) optional, Handelsname optional | only if in the record |
| MIO/FHIR variants | SNOMED CT in the KBV MIO Krankenhaus-Entlassbrief (UNVERIFIED detail) | not needed in the letter text |

## Units, numbers, dates
- Decimal comma: 1,5 mg; 38,6 °C; 184,3 mg/l. Thousands: 1.000 or thin space. Never a decimal point. BMP: "0,5" not ",5".
- Dates DD.MM.JJJJ (12.10.2026); time 14:30 Uhr; durations "7 Tage", "6 Wochen".
- Blood pressure "RR 135/80 mmHg"; heart rate "HF 88/min"; respiratory rate "AF 18/min"; oxygen saturation "SpO2 96 %" (space before %); temperature "°C".
- Lab units as in the source: Kreatinin mg/dl or µmol/l; Glukose mg/dl or mmol/l; Hb g/dl; Leukozyten /nl or /µl; CRP mg/l; HbA1c %.
- Doses: mg, µg (not mcg), g, IE (Internationale Einheiten, not IU), ml, Tropfen, Hub; forms Tabl., Filmtabl., Kps., Lsg., Inj.-Lsg., Supp., Pflaster (BMP uses "patiententaugliche Abkürzung der Darreichungsform").
- Dosierschema: morgens-mittags-abends-zur Nacht as W-X-Y-Z ("1-0-1-0"), or Freitext ("bei Bedarf", "1 x wöchentlich montags").

## Abbreviations
Common in German physician letters and acceptable in moderation (convention; no primary source forbids them). Expand on first use when the reader may be outside the specialty; never abbreviate the Hauptdiagnose text.
| Abbrev. | Meaning | English |
|---|---|---|
| Z.n. | Zustand nach | history of / status post |
| V.a. | Verdacht auf | suspected |
| DD | Differentialdiagnose | differential diagnosis |
| o.B. | ohne Besonderheiten / ohne Befund | unremarkable |
| a.e. | am ehesten | most likely |
| bds. | beidseits | bilateral |
| re./li. | rechts/links | right/left |
| i.v. / p.o. / s.c. / i.m. | intravenös / per os / subkutan / intramuskulär | routes |
| AZ / EZ | Allgemeinzustand / Ernährungszustand | general / nutritional state |
| HD / ND | Hauptdiagnose / Nebendiagnose | main / secondary diagnosis |
| AU | Arbeitsunfähigkeit | incapacity for work |
| AHB | Anschlussheilbehandlung | post-acute rehabilitation |
| MRE / MRSA | multiresistente Erreger / Methicillin-resistenter Staphylococcus aureus | |
| KHK, pAVK, COPD, aHT, DM2 | coronary disease, PAD, COPD, arterial hypertension, type 2 diabetes | fine in Nebendiagnosen with ICD code |
Avoid: English-only abbreviations (PMH, HPI, ROS, d/c, bid/tid, PRN — write "bei Bedarf"), US lab shorthand (BMP, CBC), and unexplained local ward codes.
