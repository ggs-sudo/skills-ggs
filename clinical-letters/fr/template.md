# Template — lettre de liaison à la sortie / compte rendu de consultation

Headings in French verbatim, in the order of Art. R1112-1-2 II. Body language
per task (v1: English). Replace every `<...>`. Outpatient variant: use the
alternative heading given in brackets and keep the order.

---

## En-tête (header block)

```
<Établissement> — <Service>
Statut du document : <définitif | incomplet (en attente de résultats)>
Date : <JJ/MM/AAAA>   (day of discharge, or day of consultation)

Patient : <Nom de naissance> <Prénom>, né(e) le <JJ/MM/AAAA>, sexe <F|M>
Médecin traitant : Dr <Nom>, <adresse>
Praticien adresseur : <Dr Nom, adresse | sans objet>
Rédacteur : Dr <Nom>, <fonction>, <service>, tél. <numéro>, MSSanté <adresse>
```

Rule: every field above is scored by HAS QLS criteria 4 to 7. "Statut" is
required by the ANS model. For a consultation letter add the line
`Structure : lettre de liaison (art. R1112-1-2 CSP), adaptée à une
consultation externe`.

## Titre

`Lettre de liaison à la sortie` [outpatient: `Compte rendu de consultation`]

Rule: never call an outpatient letter a lettre de liaison à la sortie
d'hospitalisation.

## Formule d'appel

`Cher Confrère, Chère Consœur,`

Rule: convention, not regulation. Keep the register formal throughout.

## 1. Identification et modalités de prise en charge

```
Hospitalisation du <JJ/MM/AAAA> au <JJ/MM/AAAA>
Mode d'entrée : <programmé | urgence | transfert>  —  Adressé par : <...>
Mode de sortie : <domicile | transfert vers ... | autre>
```

[outpatient: `Consultation du <JJ/MM/AAAA>` and `Mode d'adressage : <adressé
par le médecin traitant | autre praticien | de sa propre initiative>`]

Rule: both dates, the modes and all four identities must be present.

## 2. Motif d'hospitalisation [Motif de la consultation]

`<the referral question, 1 to 3 lines>`

Rule: state the question as it was referred, not the conclusion.

## 3. Synthèse médicale du séjour [Synthèse médicale de la consultation]

```
<Narrative of the course, grouped by pathology, each with its CIM-10 code
and its situation at discharge.>

Actes et examens : <conclusions of imaging, biology, procedures | aucun acte
| résultats en attente>

Événements indésirables : <description | aucun événement indésirable>
Micro-organismes multirésistants ou émergents : <germe, site | aucun>
Produits sanguins ou dérivés du sang : <produit, date | aucune administration>
Dispositif médical implantable : <dispositif, date, référence | aucun>

Situation clinique à la sortie : <state at discharge: autonomy, symptoms,
haemodynamics, pending issues.>
```

Rule: the four risk lines are named by the décret. Write the explicit negative
when they did not occur. The closing "situation clinique" line is required by
QLS criterion 9 and is separate from the narrative.

## 4. Traitements à la sortie [Traitements prescrits à l'issue de la consultation]

| DCI (nom commercial) | Dosage unitaire | Rythme | Voie | Durée | Statut | Motif |
|---|---|---|---|---|---|---|
| `<DCI>` | `<mg>` | `<x/j>` | `<orale>` | `<n jours \| au long cours>` | `<instauré\|modifié\|poursuivi\|arrêté>` | `<reason if not poursuivi>` |

```
Traitement habituel : <poursuivi sans modification | modifications ci-dessus |
absence de traitement habituel>
Traitements arrêtés durant le séjour : <drug — motif d'arrêt ou de remplacement>
```

Rule: QLS criterion 11 requires, per drug, DCI, dosage unitaire AND rythme,
voie AND durée. Every stopped or replaced drug needs its motif. If nothing is
prescribed write `Absence de traitement à la sortie`. Group by domaine
pathologique when the list is long, and justify the absence of a classically
recommended drug.

## 5. Résultats en attente

`<examen, date prélevée, who will receive it, and that a completed letter will
follow>` or `Aucun résultat en attente`

Rule: naming the pending result is item 5 of the décret; if anything is
pending, the header statut must read "incomplet".

## 6. Suites à donner

```
Rendez-vous : <médecin traitant: délai, RDV pris | à prendre par le patient>
             <spécialiste / examens: date, RDV pris | à prendre>
Soins infirmiers / rééducation : <prescription | sans objet>
Actions médico-sociales : <aide à domicile, assistante sociale | sans objet>
ALD : <faite | à demander | sans objet>
Surveillances particulières : <INR, kaliémie, poids, parameter + rhythm | aucune>
Point de vigilance : <oui — raison et appel à passer | non>
```

[Optional rubriques, here or inside item 3, never before item 2: antécédents,
allergies (mandatory if an adverse event occurred), mode de vie, examen
clinique, éléments remis au patient.]

Rule: every recommendation names an owner and a delay. If none is needed write
`Ne nécessite pas de soins immédiats`.

## Bloc de clôture

```
Lettre remise au patient le <JJ/MM/AAAA> <| refus du patient: motif>
Transmise le même jour au médecin traitant <et au praticien adresseur> par
MSSanté ; versée dans le DMP.

Bien confraternellement,
Dr <Nom>, <fonction>
<Service>, <Établissement> — tél. <numéro>
```

Rule: the remise and the same-day transmission lines are scored by QLS
criteria 3 and 4. Write them explicitly even when obvious.
