# Self-check: de-arztbrief (binary, one line each)

Tags: [structure] heading/order, [content] § 9 Abs. 3 items and data, [style] register and conventions, [forbidden] must be absent. Each item is pass/fail.

## Header and label
1. [structure] Document title contains exactly one of "Vorläufiger Entlassbrief" or "Endgültiger Entlassbrief".
2. [content] Patientenstammdaten present: Nachname, Vorname, Geburtsdatum (DD.MM.JJJJ).
3. [content] Aufnahmedatum and Entlassdatum both present in DD.MM.JJJJ.
4. [content] Behandelnder Krankenhausarzt named with function.
5. [content] A "Telefon für Rückfragen" / "Telefonnummer" with a number is present in the header or closing.
6. [structure] Addressee is a Hausarzt / weiterbehandelnder Arzt (named or "An: Hausarztpraxis").
7. [content] If labelled vorläufig, the letter names the outstanding items and states that an endgültiger Entlassbrief follows.

## Section headings and order
8. [structure] Heading "Anrede" content present: "Sehr geehrte Frau Kollegin" / "Sehr geehrter Herr Kollege" (or combined) opens the letter body.
9. [structure] Headings appear in this relative order: Grund der Einweisung → Diagnosen → Anamnese → Befunde → Entlassungsbefund → Epikrise → Weiteres Prozedere/Empfehlungen → Medikation bei Entlassung → Veranlasste Leistungen und Arbeitsunfähigkeit → Nachfolgende Versorgungseinrichtung → Mitgegebene Befunde → Abschließende Bemerkungen.
10. [structure] Heading "Grund der Einweisung" present.
11. [structure] Heading "Diagnosen" present.
12. [structure] Heading "Allergien/Unverträglichkeiten" present (may be "keine bekannt").
13. [structure] Heading "Anamnese" present.
14. [structure] Heading "Befunde" present.
15. [structure] Heading "Entlassungsbefund" present.
16. [structure] Heading is exactly "Epikrise" (not "Zusammenfassung", "Verlauf", "Hospital course").
17. [structure] Heading "Weiteres Prozedere/Empfehlungen" present.
18. [structure] Heading "Medikation bei Entlassung" present.
19. [structure] Heading "Veranlasste Leistungen und Arbeitsunfähigkeit" present.
20. [structure] Heading "Nachfolgende Versorgungseinrichtung" present.
21. [structure] Heading "Mitgegebene Befunde" present.
22. [structure] Heading "Abschließende Bemerkungen" present and is the last section.

## Content of the 12 binding items
23. [content] Grund der Einweisung states the reason at admission (symptom or referral question), not only the final diagnosis.
24. [content] Diagnosen list has a Hauptdiagnose first, then Nebendiagnosen.
25. [content] Every diagnosis carries an ICD-10-GM code in parentheses after the text.
26. [content] A line on multiresistente Erreger exists (positive finding or "kein Nachweis").
27. [content] Allergien/Unverträglichkeiten names substances and reactions, or "keine bekannt".
28. [content] Anamnese includes Medikation bei Aufnahme with Stärke and Dosierschema (or states "keine Dauermedikation").
29. [content] Befunde carry dates and values with units.
30. [content] Entlassungsbefund describes clinical state at discharge (vitals or functional status).
31. [content] Epikrise covers Anamnese, Diagnostik, Therapie and Prozeduren in prose and interprets the course.
32. [content] Weiteres Prozedere has at least one concrete request to the Hausarzt with a date or interval.
33. [content] Weiteres Prozedere states "Ausstehende Befunde: …" or "keine".
34. [content] Each discharge drug line has Wirkstoff, Stärke, Darreichungsform, Dosierschema and Therapiedauer.
35. [content] Each drug line carries a status (neu / geändert / unverändert / abgesetzt).
36. [content] Every neu, geändert or abgesetzt drug has a Begründung.
37. [content] A Medikationsplan table exists with the BMP columns Wirkstoff, Handelsname, Stärke, Form, Mo, Mi, Ab, zN, Einheit, Hinweise, Grund.
38. [content] Medikationsplan rows are grouped under BMP Zwischenüberschriften (Dauermedikation, Bedarfsmedikation, zeitlich befristet …, Selbstmedikation) where more than one group applies.
39. [content] "Mitgegebene Arzneimittel" line present (list or "keine").
40. [content] Verordnungen line present (list or "keine").
41. [content] Arbeitsunfähigkeit line present ("AU-Bescheinigung ausgestellt bis DD.MM.JJJJ" or "entfällt" with reason).
42. [content] Nachfolgende Versorgungseinrichtung names a setting (häusliches Umfeld / Reha / Pflegeeinrichtung).
43. [content] Mitgegebene Befunde lists documents or "keine".
44. [content] Every statement traces to the record; unknown values are written as "nicht dokumentiert", not invented.

## Style and conventions
45. [style] Sie-form throughout; the reader is the colleague, not the patient.
46. [style] Closing contains "Für Rückfragen stehen wir Ihnen … zur Verfügung" and a Grußformel ("Mit freundlichen kollegialen Grüßen" or "Mit kollegialen Grüßen").
47. [style] At least one signature line with name and function (Oberarzt/-ärztin, Chefarzt/-ärztin, Stationsarzt/-ärztin).
48. [style] All dates DD.MM.JJJJ; no YYYY-MM-DD, no MM/DD/YYYY, no month names in English.
49. [style] Decimal comma in all numeric values (38,6 °C; 1,5 mg); no decimal points.
50. [style] Every Dosierschema has four filled positions (e.g. 1-0-1-0) or is a Freitext such as "bei Bedarf"; no blank position, no ",5".
51. [style] Drugs named by Wirkstoff (INN); Handelsname at most in parentheses.
52. [style] Headings are German; body may be English (v1) but headings, labels, Anrede and Grußformel are German.
53. [style] Anamnese, Epikrise and Weiteres Prozedere are prose or dated requests, not bare keyword fragments.
54. [style] Abbreviations Z.n., V.a., o.B. appear only in Nebendiagnosen/body, never in the Hauptdiagnose text.

## Forbidden
55. [forbidden] No second label (both vorläufig and endgültig) and no missing label.
56. [forbidden] No heading from another national format: "Kern", "Dossiersamenvatting", "Hospital course", "Discharge summary", "Plan and requested actions", "Résumé", "Suites à donner".
57. [forbidden] No drug named by brand only, no dose without Stärke and Dosierschema.
58. [forbidden] No binding item silently omitted; absence is written as "keine" / "entfällt".
59. [forbidden] No patient-facing instructions ("Sie sollten …" to the patient) inside the physician letter.
60. [forbidden] No real patient identifiers, no invented lab values, no diagnosis stated as certain when the record says V.a.
