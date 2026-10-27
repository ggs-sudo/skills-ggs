# Template: ontslagbericht (Richtlijn HASP, 3rd ed. 2017)

Keep the three parts and the rubriek order exactly. `*` = mandatory: always
print the rubriek; write `geen` if there is nothing to report. `***` =
mandatory for kwetsbare ouderen (frail elderly). Unmarked rubrieken are
optional and may be left out. Replace <placeholders>; keep Dutch rubriek names,
drop the English in parentheses in the final letter.

## Envelop

**Gegevens auteur\*** (author)
<Hospital name, address, phone> / <Dr. Initials Surname (specialism)> /
contactpersoon: <name, role, phone, e-mail, availability e.g. ma-vr 9-17 uur>
Rule: institution, responsible specialist, and when/how the contact is reachable.

**Gegevens patiënt of cliënt\*** (patient)
<Surname, initials> <BSN> (<m/v>) <DD-MM-JJJJ> / <address> / contactpersoon: <name (relation), phone>
Rule: BSN, name, sex, date of birth, address; contactpersoon when relevant.

**Gegevens geadresseerde\*** (addressee)
<Practice or institution, address, phone, e-mail> / <Name (huisarts)>
Rule: discharge home = the huisarts; discharge to an institution = that institution, huisarts as copy.

**Gegevens kopie-ontvanger(s)** (copy recipients)
<Name, role, institution> or omit
Rule: mandatory copy to the huisarts when the addressee is another institution.

**Datum en tijd\*** (date and time)
<DD-MM-JJJJ HH:MM>
Rule: moment the sender authorises the message.

**Type bericht\*** (message type)
<ontslagbericht kliniek | ontslagbericht polikliniek>
Rule: use exactly one of the four HASP values (also: update kliniek, update polikliniek).

**Zorgpad** (care pathway) <only if regionally agreed>
**Urgentie** (urgency) <only if regionally agreed>

**Beheerder bericht\*** (message custodian)
<Hospital name>
Rule: the organisation that archives the message, usually the sender.

## Kern

**Reden bericht\*** (reason for message)
Kliniek: Ontslag naar <huis/instelling>. De patiënt was bij ons opgenomen <via verwijzing/via de spoedeisende hulp> van <DD-MM-JJJJ> tot <DD-MM-JJJJ> in verband met <reason>.
Polikliniek: Ontslag uit poliklinische controle. Laatste bezoek was <DD-MM-JJJJ>. U verwees patiënt in verband met <referral reason>.
Rule: always how long, for what, by which route, and where the patient goes now.

**Conclusie, diagnose\*** (conclusion, diagnosis)
1. <diagnosis or working hypothesis, with your current judgement, response to treatment, prognosis if known>
2. <...>
Rule: compact; answer the referral question; no explanatory detail (that goes in the Dossiersamenvatting); frail elderly: state whether a delier occurred.

**Beleid\*** (management)
Ad 1. <what was done and is now current; exactly which drug was stopped/lowered/started/raised; which diagnostics are still open>
Ad 2. <...>
Rule: changes and open items only; no dose schedules here, they go in Medicatie.

**Aanbeveling uw follow-up\*** (recommended follow-up by you)
Ad 1. <which checks, when, what they consist of; continue or stop which medication; referral advice>
Ad 2. <...>
Rule: addressed to the receiver; include advice from consulting specialties; if none, write `geen`.

**Afgesproken met patiënt** (agreed with patient)
<who makes which appointment; what the patient was told; direct ward contact allowed until <date>>
Rule: the responsibility agreed with the patient; must be consistent with Beleid and Aanbeveling uw follow-up.

**Verder van belang** (also of note)
<a few words, or "Zie <rubriek>." pointing into the Dossiersamenvatting>
Rule: only for something the GP must not overlook; otherwise omit.

## Dossiersamenvatting

**Voorgeschiedenis** (past history)
<JJJJ diagnosis/procedure, one per line, only what relates to this episode>

**Anamnese** (history)
<DD-MM-JJJJ> <relevant findings; state "heteroanamnese" if from a third party>

**Beloop, interventie** (course, intervention)
<DD-MM-JJJJ> <key points of the course, procedures, therapeutic diagnostics>

**Familieanamnese** (family history)
<disease and family relation, e.g. "vader: myocardinfarct op 58 jaar">

**Psychosociale anamnese** (psychosocial history)
<only when it adds value for the GP>

**Risicovol leefgedrag\*** (risk behaviour)
<tobacco, alcohol, drugs, injecting, sexual risk; include negative findings if asked; else `geen`>

**Lichamelijk onderzoek** (physical examination)
<DD-MM-JJJJ> <relevant positive and negative findings with values and units>

**Laboratoriumonderzoek** (laboratory)
<DD-MM-JJJJ> <test> <value> <unit> (<reference>) per line; date, place, type, material, value
Rule: dated; units stated; relevant results only.

**Beeldvormend onderzoek** (imaging)
<DD-MM-JJJJ> <modality>: <conclusion>

**Functieonderzoek** (functional tests)
<DD-MM-JJJJ> <ECG, lung function, vascular, hearing: conclusion>

**Psychogeriatrisch onderzoek\*\*\*** (psychogeriatric assessment)
<cognitie / somatisch / functioneel / sociaal, with dated scores> or omit if not frail elderly

**Overig aanvullend onderzoek** (other investigations)
<DD-MM-JJJJ> <cultures, antigen tests, skin tests, etc.>

**Intercollegiale consulten** (consultations)
<DD-MM-JJJJ> <specialty>: <conclusion>; consult geriater always listed

**Verrichtingen derden** (procedures by third parties)
<DD-MM-JJJJ> <procedure, by whom> or omit

**Medicatie\*** (medication)
<DD-MM-JJJJ start> <drug> <form> <strength> <dose, e.g. 1 dd 1> <oral/inhalation> [gewijzigd/nieuw]
Gestopt: <DD-MM-JJJJ> <drug> <reason>
Rule: the full current list as known to the sender at sending; stopped drugs with reason; else `geen`.

**Overgevoeligheid voor medicatie; contra-indicaties voor voorschrijven\*** (hypersensitivity; contraindications)
<DD-MM-JJJJ> <agent>, aard reactie: <...>, ernst: <...>, vaststeller: <...>; <contraindication> or `geen bekend`

**Profylaxe\*** (prophylaxis)
<DD-MM-JJJJ> <measure and indication, e.g. endocarditis prophylaxis, BRMO precautions> or `geen`

**Behandelgrenzen\*\*\*** (treatment limits)
Besproken <DD-MM-JJJJ> met <patient, relatives, doctor>: <reanimatie ja/nee; ic-opname ja/nee; beademing ja/nee; ...>
Rule: exactly which agreement, with whom, when; mandatory for frail elderly, otherwise include when discussed.
