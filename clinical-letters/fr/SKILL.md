---
name: fr-lettre-de-liaison
description: Write the French hospital letter to the médecin traitant (lettre de liaison à la sortie, compte rendu d'hospitalisation or compte rendu de consultation) in the structure required by Art. R1112-1-2 Code de la santé publique and scored by the HAS QLS indicator. Use for France, a French hospital, "letter to the GP in France", lettre de liaison, médecin traitant. Read template.md for heading order and checklist.md before finishing.
---

# Lettre de liaison à la sortie (France)

## 1. Scope and addressee
- Legal object: lettre de liaison à la sortie, written by "le médecin de l'établissement qui l'a pris en charge" (Art. R1112-1-2 I CSP, Décret n° 2016-995 du 20/07/2016, in force 01/01/2017). HAS: it "remplace le compte rendu d'hospitalisation et la lettre rédigée à l'occasion de la sortie". One document; no short letter followed by a CRH.
- Handover: "remise au patient" by the physician or a team member "qui s'assure que les informations utiles à la continuité des soins ont été comprises" (R1112-1-2 I); or, with consent, to the personne de confiance (L1112-1). The patient reads it: write for a confrère, nothing you would not hand to the patient.
- Transmission: "transmise le même jour, au médecin traitant et, le cas échéant, au praticien qui a adressé le patient", by "messagerie sécurisée" (MSSanté) "ou par tout moyen garantissant la confidentialité", and "versée dans le dossier médical partagé" (DMP) if it exists (R1112-1-2 I).
- Dating: HAS QLS criterion 2 scores the letter 0 unless dated the day of discharge.
- Our inputs are outpatient consultations; the décret covers hospitalisation. Apply section 5 and label the adaptation.

## 2. The six regulatory items, in this order (R1112-1-2 II)
"Cette lettre de liaison contient les éléments suivants :"
1. "Identification du patient, du médecin traitant, le cas échéant du praticien adresseur, ainsi que l'identification du médecin de l'établissement de santé qui a pris en charge le patient avec les dates et modalités d'entrée et de sortie d'hospitalisation" (identification; dates and modes of admission/discharge). QLS: patient = nom de naissance ET prénom ET date de naissance ET sexe (crit. 5); médecin traitant = nom ET adresse (crit. 4); signatory = nom ET service ET hôpital ET coordonnées (crit. 7); both dates (crit. 6). Mode d'entrée: programmé / urgence / transfert, and who referred.
2. "Motif d'hospitalisation" (reason for admission). Free text, 1–3 lines, the question as referred.
3. "Synthèse médicale du séjour précisant le cas échéant, les événements indésirables survenus pendant l'hospitalisation, l'identification de micro-organismes multirésistants ou émergents, l'administration de produits sanguins ou dérivés du sang, la pose d'un dispositif médical implantable" (medical summary; adverse events, MDRO, blood products, implants). QLS crit. 9 needs BOTH the course AND "une synthèse de la situation clinique du patient à sa sortie". HAS 2014: each pathology "et leur situation à la sortie" (add CIM-10); relevant normal and abnormal results of actes, examens complémentaires et biologiques (crit. 10 accepts a conclusion, "aucun acte", or "résultats en attente"). State the four risk items when present; otherwise one line saying none occurred.
4. "Traitements prescrits à la sortie de l'établissement (ou ordonnances de sortie) et ceux arrêtés durant le séjour et le motif d'arrêt ou de remplacement, en précisant, notamment pour les traitements médicamenteux, la posologie et la durée du traitement" (discharge treatments; stopped/replaced treatments with reason; posology and duration). QLS crit. 11: per drug "sa dénomination (DCI et/ou nom commercial), sa posologie (dosage unitaire ET rythme d'administration), sa voie d'administration ET sa durée", or "absence de traitement à la sortie"; AND "suppression, modification ou poursuite du traitement habituel" or "absence de traitement habituel". HAS 2014: group by domaine pathologique; justify every difference from the pre-admission treatment; flag "essai thérapeutique"; justify non-prescription of a classically recommended drug so it is not read as an omission (also ANS 3.2.7). Use the table in [template.md](template.md).
5. "Annonce, le cas échéant, de l'attente de résultats d'examens ou d'autres informations qui compléteront cette lettre de liaison" (pending results that will complete the letter). Name them and announce the completed version (HAS 2014: statut "incomplet", completed CRH within 8 days, 14 if stated). Else "Aucun résultat en attente".
6. "Suites à donner, le cas échéant, y compris d'ordre médico-social, tels que les actes prévus et à programmer, recommandations et surveillances particulières" (follow-up incl. medico-social; planned acts; recommendations; monitoring). HAS 2014 / QLS crit. 12: RDV médicaux incl. médecin traitant and examens, each "RDV pris" or "à prendre par le patient"; soins infirmiers / rééducation; actions médico-sociales; ALD faite ou à demander; "point de vigilance : oui/non" (oui = a call between teams is needed); surveillances particulières (AVK, diurétiques, chimiothérapie). Or "ne nécessite pas de soins immédiats".

Optional rubriques (HAS 2014): antécédents, allergies / événements indésirables (mandatory if one occurred), mode de vie, examen clinique, éléments remis au patient. Place inside item 3 or after item 6, never before item 2.

## 3. Quality bar: HAS QLS 2022 (12 criteria, target 80/100)
Every criterion is a numbered line in [checklist.md](checklist.md); walk it before finishing. Two it is easy to lose: the handover to the patient and the same-day transmission to the médecin traitant each need their own explicit line in the closing block.

## 4. Structural model: ANS CI-SIS LDL-SES V2020.01 (CDA, LOINC 11490-0)
Always printed [1..1]: Statut du document, Motif, Modalités d'entrée/sortie with the Synthèse médicale du séjour, Traitements à la sortie. Optional [0..1]: Traitements arrêtés durant le séjour, Résultats attendus, Suites à donner, Dispositifs médicaux, Allergies. Write "aucun" rather than dropping a mandatory section.

## 5. Adaptation to an outpatient specialist consultation (labelled)
No statute or HAS text fixes the structure of the compte rendu de consultation (none found; UNVERIFIED). The duty exists: Code de déontologie Art. R4127-58 (as amended by Décret n° 2026-691 du 27/07/2026, CNOM text): the consulted physician "doit, sauf opposition du patient, informer dans les meilleurs délais le médecin traitant ... et leur faire part de ses constatations et décisions. Il consigne la transmission dans le dossier médical"; Art. R4127-62: "toutes informations nécessaires pour le suivi du patient".
Rule: keep the six items and their order; swap vocabulary. Title "Compte rendu de consultation" + the line "Structure : lettre de liaison (art. R1112-1-2 CSP), adaptée à une consultation externe". Mapping: dates/modalités d'entrée et de sortie → date de la consultation + mode d'adressage (adressé par le médecin traitant / autre praticien / de sa propre initiative); Motif d'hospitalisation → Motif de la consultation; Synthèse médicale du séjour → Synthèse médicale de la consultation, ending with the situation clinique à l'issue de la consultation (risk items only if an act was done); Traitements prescrits à la sortie → Traitements prescrits à l'issue de la consultation, with arrêtés / modifiés + motif; items 5 and 6 unchanged. Date = consultation day; same-day transmission; remise au patient stated. Never call it a "lettre de liaison à la sortie d'hospitalisation".

## 6. Style
- v1: French headings exactly as in [template.md](template.md), body in English. In French: formal register, vouvoiement.
- Frame (professional convention, UNVERIFIED): "Cher Confrère, Chère Consœur," ... "Bien confraternellement," + signature block. Patient = "M./Mme <Nom>" or "votre patient(e)".
- Facts and decisions only; no pasted notes. Expand abbreviations at first use ([terminology.md](terminology.md)). Statut per drug: poursuivi / modifié / arrêté / instauré.

## 7. Coding, units, dates
- CIM-10 after each pathology (ANS codes problems in CIM-10). Drugs in DCI, nom commercial optional in brackets (QLS). Procedures in French, CCAM code if known (CCAM not verified in sources read, UNVERIFIED).
- Dates JJ/MM/AAAA. Laboratory units as French labs report them: créatinine µmol/L, glycémie mmol/L (g/L also used), hémoglobine g/dL (g/L in some labs) (conventions, UNVERIFIED). Convert US units and MM/DD/YYYY dates from the source.

## 8. Forbidden
- Drug line without DCI, dose ET rythme, voie, durée; stopped/replaced drug without motif; silence on traitement habituel.
- Omitting item 5 when results are pending; incomplete letter without statut.
- Date other than discharge/consultation day; missing remise au patient or transmission line.
- Labels from other national formats (Kern, Epikrise, Hospital Course, Dossiersamenvatting).
- Invented values or identifiers (RPPS, INS), real patient data; calling an outpatient letter a lettre de liaison à la sortie without the adaptation line.

## 9. Header metadata
Établissement, service, rédacteur (nom, fonction, téléphone, MSSanté); date de rédaction; patient (nom de naissance, prénom, date de naissance, sexe); médecin traitant (nom, adresse); praticien adresseur; dates et modalités or date de consultation + mode d'adressage; statut du document; liste de diffusion; personne de confiance (optional).

## 10. Self-check
Run [checklist.md](checklist.md) line by line before finishing; compare with [example.md](example.md).

## 11. Sources read
Art. R1112-1-2 and L1112-1 CSP as quoted in HAS QLS fiche 2022 (item 4° completed from MACSF; Legifrance unreachable from this session; R1112-1-1 content from MACSF, UNVERIFIED). HAS, Document de sortie d'hospitalisation > 24h, contenu métier + fiche d'utilisation, 15/10/2014. HAS, Fiche descriptive IQSS QLS MCO, V.03/2022. ANS, CI-SIS Volet LDL-SES V2020.01, 29/04/2020. CNOM, Code de déontologie Art. 58, 60, 62, 63 (site 20/10/2026; PDF ed. 02/2021).
