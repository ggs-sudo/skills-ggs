# Checklist — France

Walk every line before finishing. Each is binary. Tags: [structure] heading
and order, [content] required facts, [style] register and conventions,
[forbidden] must not appear.

## Header and identification

1. [structure] A `Statut du document` line is present and reads `définitif` or `incomplet`.
2. [content] The date is the day of discharge, or of the consultation (QLS criterion 2).
3. [content] Patient is identified by nom de naissance, prénom, date de naissance and sexe (QLS 5).
4. [content] Médecin traitant is identified by name and address (QLS 4).
5. [content] Praticien adresseur is named, or explicitly `sans objet`.
6. [content] The hospital physician is identified by name, fonction, service, établissement and a contact number (QLS 7).
7. [content] Admission and discharge dates are both present; for an outpatient letter, the consultation date (QLS 6).
8. [content] Mode d'entrée and mode de sortie are stated, or for an outpatient letter the mode d'adressage.
9. [structure] The title is `Lettre de liaison à la sortie`, or `Compte rendu de consultation` for an outpatient letter.
10. [structure] An outpatient letter carries the line `Structure : lettre de liaison (art. R1112-1-2 CSP), adaptée à une consultation externe`.

## Order and completeness of the six items

11. [structure] The six numbered items appear in the order of Art. R1112-1-2 II.
12. [structure] All six headings use the French wording from template.md verbatim.
13. [structure] No optional rubrique (antécédents, allergies, mode de vie, examen clinique) appears before item 2.
14. [structure] No heading has been added that is not in template.md.

## Item 2, motif

15. [content] The motif states the referral question, not the conclusion.

## Item 3, synthèse

16. [content] Each pathology carries a CIM-10 code.
17. [content] Each pathology states its situation at discharge.
18. [content] `Actes et examens` gives conclusions, or `aucun acte`, or `résultats en attente` (QLS 10).
19. [content] `Événements indésirables` is answered, positively or with the explicit negative.
20. [content] `Micro-organismes multirésistants ou émergents` is answered.
21. [content] `Produits sanguins ou dérivés du sang` is answered.
22. [content] `Dispositif médical implantable` is answered.
23. [content] A distinct closing line gives the `Situation clinique à la sortie` (QLS 9).

## Item 4, treatments

24. [content] Every drug line carries DCI, dosage unitaire, rythme, voie and durée (QLS 11).
25. [content] Every drug carries exactly one statut: instauré, modifié, poursuivi or arrêté.
26. [content] Every `modifié` and every `arrêté` drug carries a motif.
27. [content] A `Traitement habituel` line states suppression, modification, poursuite, or absence (QLS 11).
28. [content] `Traitements arrêtés durant le séjour` lists stopped or replaced drugs with their motif, or is `sans objet`.
29. [content] If nothing is prescribed, the letter says `Absence de traitement à la sortie`.
30. [content] Where a classically recommended drug is not prescribed, the reason is given.

## Item 5, pending results

31. [content] Pending results are named individually, with who receives them and that a completed letter follows.
32. [content] If nothing is pending, the letter says `Aucun résultat en attente`.
33. [structure] If anything is pending, the header statut reads `incomplet`.

## Item 6, follow-up

34. [content] Every appointment states a delay or a date and whether it is `RDV pris` or `à prendre par le patient`.
35. [content] Soins infirmiers / rééducation is answered, or `sans objet`.
36. [content] Actions médico-sociales is answered, or `sans objet`.
37. [content] ALD is answered: faite, à demander, or sans objet.
38. [content] Surveillances particulières names each parameter and its rhythm, or `aucune`.
39. [content] A `Point de vigilance` line reads `oui` with a reason, or `non`.
40. [content] If no follow-up is needed, the letter says `Ne nécessite pas de soins immédiats`.

## Closing block

41. [content] A line states the letter was handed to the patient, with the date, or records a refusal and its motif (QLS 3).
42. [content] A line states same-day transmission to the médecin traitant, the channel used, and the DMP deposit (QLS 4).
43. [style] The letter closes with a signature block naming the author, service, établissement and telephone number.

## Style

44. [style] Formal register throughout; vouvoiement; opening and closing formulae present.
45. [style] Every abbreviation is expanded at first use.
46. [style] Dates are `JJ/MM/AAAA`; the decimal separator in French text is a comma.
47. [style] Laboratory values use French units, with the source unit converted.
48. [style] Every clinical statement traces to a retrieved record entry.

## Forbidden

49. [forbidden] No drug line missing dose, rythme, voie or durée.
50. [forbidden] No stopped or replaced drug without a motif.
51. [forbidden] No silence on the traitement habituel.
52. [forbidden] No heading or label from another national format (Kern, Beleid, Epikrise, Hospital Course, Dossiersamenvatting, Stamdata).
53. [forbidden] No invented identifier (RPPS, INS, MSSanté address) and no real patient data.
54. [forbidden] An outpatient letter is never called a lettre de liaison à la sortie d'hospitalisation.
55. [forbidden] No placeholder `<...>` left in the finished letter.
56. [forbidden] No pasted ward notes or raw laboratory dumps.
