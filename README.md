# XKaliber

**The assessment that reveals true calibre.**

XKaliber is the adaptive competency assessment engine of **CertifiKation**, within **KonnectED**, a module of **Konnaxion**.

This repository is intentionally **technology-agnostic**. It does not prescribe any framework, programming language, database, or provider. It serves as a product, functional, architectural, and governance starting point for designing the application before technical choices are made.

## Core idea

A uniform test mostly measures how well someone fits the test. XKaliber instead measures the level at which a person remains reliably competent.

The system starts by validating existing knowledge and skills, then gradually adjusts difficulty to reveal:

- what the person can perform comfortably;
- the threshold at which their competency remains reliable;
- the upper boundary worth exploring;
- areas of uncertainty;
- evidence that can be exported to CertifiKation;
- structured competency evidence that can be routed through **K-Port** to **EkoH** for domain-bounded reputation processing within Konnaxion.

## Brand metaphor

In the myth, Excalibur is the trial that reveals who is capable of carrying a role.

Within Konnaxion, **XKaliber** becomes the assessment that reveals which competency, responsibility, or decision a person is equipped to carry.

The Round Table becomes operational: people are not merely heard; their competencies are situated, their expertise is bounded by domain, and collective governance can rely on explicit evidence rather than status, noise, or popularity.

## Repository structure

```text
xkaliber-starter/
├─ README.md
├─ BRAND.md
├─ PRODUCT_BRIEF.md
├─ ROADMAP.md
├─ PROJECT_BOARD.md
├─ GOVERNANCE.md
├─ CONTRIBUTING.md
├─ SECURITY_AND_PRIVACY.md
├─ LICENSE.md
├─ docs/
│  ├─ architecture/
│  ├─ evaluation/
│  ├─ governance/
│  ├─ product/
│  ├─ ux/
│  └─ integration/
├─ contracts/
├─ examples/
├─ tests/
│  └─ acceptance/
└─ decisions/
```

## Design principles

XKaliber must remain:

1. **adaptive** — difficulty changes according to performance;
2. **explainable** — the person understands how their profile is produced;
3. **governable** — rules, thresholds, and weightings are visible and revisable;
4. **domain-bounded** — a validated competency does not grant general authority;
5. **useful** — results support learning, hiring, certification, or guidance;
6. **contestable** — errors, bias, and anomalies must be reviewable;
7. **exportable** — assessment evidence can flow into CertifiKation and, through K-Port, into EkoH and the wider Konnaxion ecosystem.

## Integration boundary

XKaliber is responsible for **measuring competency and producing assessment evidence**. It does not calculate a person's final reputation or authority within Konnaxion.

The intended flow is:

```text
XKaliber
   ↓
Calibre Profile
   ↓
CertifiKation evidence
   ↓
K-Port
   ↓
EkoH
   ↓
Governed downstream use in Konnaxion
```

**CertifiKation** attests the XKaliber result. **K-Port** is the canonical evidence gateway: it validates provenance, status, scope, consent, and domain mapping without re-scoring the XKaliber assessment. **EkoH** is responsible for transforming qualified evidence into domain-bounded reputation signals.

## Initial MVP objective

Create an initial version capable of:

- defining domains and competencies;
- launching a simple adaptive assessment;
- adjusting difficulty after each block of questions or tasks;
- producing a Calibre Profile;
- generating CertifiKation evidence;
- explaining the result to the assessed person and the organization;
- recording assessment decisions in an auditable manner;
- exporting structured assessment evidence for ingestion by K-Port.

## Decisions not to make too early

This repository intentionally avoids choosing:

- programming language;
- front-end framework;
- database;
- AI provider;
- cloud infrastructure;
- final identity protocol;
- final certificate format.

These choices should be made only after validating the needs, workflows, competency model, integration boundaries, and required level of evidence.
