# clinical-letters skills

Skills for writing a hospital doctor's letter to the patient's general
practitioner in a national format. Built for the skills experiment described in
`../../proposal.md`. Served to agents through the mcp-gateway skills server.

## Layout

```
clinical-letters/
  core/SKILL.md                 shared grounding, medication and safety rules
  <country>/SKILL.md            structure, headings, language, conventions
  <country>/template.md         heading skeleton in required order
  <country>/example.md          one synthetic worked letter
  <country>/terminology.md      terms, code systems, units, dates
  <country>/checklist.md        binary checks mirrored by the grader
```

Countries: `dk` (epikrise, STPS VEJ 10036), `nl` (ontslagbericht, Richtlijn
HASP), `de` (Arztbrief / Entlassbrief, Rahmenvertrag Entlassmanagement § 9 and
HL7 DE Arztbrief Plus), `uk` (PRSB eDischarge Summary and Outpatient Letter),
`fr` (lettre de liaison à la sortie, Art. R1112-1-2 CSP).

## What each skill enforces

The structures diverge enough for a deterministic grader to tell them apart.

| | First substantive section | Medication placement | Order fixed by |
|---|---|---|---|
| dk | Anbefaling om opfølgning hos egen læge (mandated first) | Medicinliste mandated last | Vejledning for first and last only |
| nl | Kern: Reden bericht → Conclusie → Beleid → Aanbeveling uw follow-up | Changes in Beleid, prescriptions in Dossiersamenvatting | Guideline fixes all three parts |
| de | Grund der Einweisung, then Diagnosen | Medikation bei Entlassung near the end, plus Medikationsplan | 12 items binding, order conventional |
| uk | Patient demographics, then Clinical summary (both Mandatory) | Medications and Medical Devices, with change status | Order is a local decision; skill picks a default |
| fr | 1. Identification, 2. Motif | 4. Traitements à la sortie, table with DCI/posologie/voie/durée | Six numbered items fixed by decree |

Distinctive testable rules: dk forbids the word "foreløbig" and carries a
Rød/Gul/Grøn/Hvid follow-up marking; nl prints mandatory rubrieken even when
empty, with the literal "geen"; de labels every letter "vorläufig" or
"endgültig" and gives a callback number; uk tags each heading Mandatory,
Required or Optional; fr needs an explicit handover and same-day transmission
line for the HAS quality indicator.

## Validation

`python3 ../../validate_skills.py` checks every bundle against the gateway's
rules: frontmatter keys, tool-name collisions after slugification, the 10,000
character body cap, the 1 MB fetch limit, broken relative links, leftover
placeholders, a Sources section, and that each SKILL.md links its template and
checklist. All six bundles pass as of 2026-10-26.

## Rules for authors

- Every normative statement in a SKILL.md comes from a primary source listed in
  its Sources section. Unverified items are marked (UNVERIFIED).
- Frontmatter has exactly `name` and `description`. The gateway mints the tool
  `read_skill_<slugified name>` and uses `description` as the tool description,
  so the description carries the trigger phrases.
- Sub-resources are referenced with relative markdown links. The gateway
  parses those links and returns them as `path` values the agent can pass back.
- Examples are synthetic. No real patient data anywhere in this tree.
- Files stay well under the gateway's 1 MB per-file limit.

## Serving

The gateway fetches public HTTPS URLs only, so this tree must be hosted
somewhere public. With a raw GitHub base `<RAW>`, one connector carries up to
five skills:

```
http://mcp-gateway.shared:80/skills/mcp?url=<RAW>/clinical-letters/core/SKILL.md,<RAW>/clinical-letters/dk/SKILL.md,<RAW>/clinical-letters/nl/SKILL.md,<RAW>/clinical-letters/de/SKILL.md,<RAW>/clinical-letters/uk/SKILL.md
```

`fr` needs a second connector or replaces one of the above.
