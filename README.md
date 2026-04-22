# WITNESS DATA FACTORY™

**Zero-PHI. Trinity-certified. Synthetic medical datasets for clinical AI.**

[![Platform](https://img.shields.io/badge/Platform-Live-brightgreen)](https://witness-data-factory.onrender.com)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-WitnessDataFactory-yellow)](https://huggingface.co/WitnessDataFactory)
[![License](https://img.shields.io/badge/License-Commercial-blue)](mailto:WitnessDataFactory@gmail.com)
[![QA Gate](https://img.shields.io/badge/Trinity%20QA%20Gate-97%25-brightgreen)](https://witness-data-factory.onrender.com)

---

## ⚡ Get Started in 60 Seconds

**Free 1,000-record samples. No card. No NDA. No IRB wait.**

| Domain | Browse Sample | Live Download |
|---|---|---|
| Oncology | [oncology_sample_1k.csv](samples/oncology/oncology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/oncology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=oncology_1k) |
| Cardiology | [cardiology_sample_1k.csv](samples/cardiology/cardiology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/cardiology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=cardiology_1k) |
| Neurology | [neurology_sample_1k.csv](samples/neurology/neurology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/neurology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=neurology_1k) |
| Pathology | [pathology_sample_1k.csv](samples/pathology/pathology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/pathology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=pathology_1k) |
| Radiology | [radiology_sample_1k.csv](samples/radiology/radiology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/radiology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=radiology_1k) |
| Endocrinology | [endocrinology_sample_1k.csv](samples/endocrinology/endocrinology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/endocrinology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=endocrinology_1k) |
| Pharmacology | [pharmacology_sample_1k.csv](samples/pharmacology/pharmacology_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/pharmacology?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=pharmacology_1k) |
| Rare Disease | [rare_disease_sample_1k.csv](samples/rare_disease/rare_disease_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/rare_disease?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=rare_disease_1k) |
| Surgical | [surgical_sample_1k.csv](samples/surgical/surgical_sample_1k.csv) | [Download 1k records →](https://witness-data-factory.onrender.com/free-sample/surgical?utm_source=github_public&utm_medium=readme&utm_campaign=get_started&utm_content=surgical_1k) |

> Paid packs (10k → 1M records) delivered instantly via Stripe + presigned download URL.
> [**Order now →**](https://witness-data-factory.onrender.com?utm_source=github_public&utm_medium=readme&utm_campaign=enterprise&utm_content=paid_tiers)

---

## Repository Structure

```
witness-data-public/
├── samples/                        # Free 1k preview records per domain (CSV)
│   ├── oncology/
│   ├── cardiology/
│   ├── neurology/
│   ├── pathology/
│   ├── radiology/
│   ├── endocrinology/
│   ├── pharmacology/
│   ├── rare_disease/
│   └── surgical/
├── schemas/                        # JSON Schema definitions for all 9 domains
│   ├── oncology_schema.json
│   ├── cardiology_schema.json
│   └── ... (all 9 domains)
├── certificates/                   # QA certificate format + example
│   └── README.md
└── docs/
    ├── quickstart.md               # Python load, validate, HuggingFace examples
    ├── compliance.md               # HIPAA / GDPR / EU AI Act details
    └── schema_overview.md          # All 9 domain label fields reference
```

---

## What Is WITNESS DATA FACTORY™

Medical AI teams waste months on IRB approvals, de-identification workflows, and legal reviews just to access fragmented, incomplete records.

We eliminate that wait entirely.

WITNESS DATA FACTORY™ is a deterministic GenAI pipeline that generates, validates, and delivers **production-grade synthetic clinical text datasets** — certified under a 97% Trinity Ensemble consensus gate — with zero real patient data ever accessed or stored.

**The factory produces the datasets. The datasets are the product.**

---

## Nine Clinical Domains

| Domain | Focus |
|---|---|
| `oncology` | Tumor triage, chemotherapy notes, staging reports |
| `cardiology` | Medication management, cardiac event documentation |
| `neurology` | Cognitive assessments, neurological event records |
| `pathology` | Specimen reports, biopsy findings, histology notes |
| `radiology` | Imaging interpretation, scan reports, findings |
| `endocrinology` | Metabolic condition records, hormone management |
| `pharmacology` | Drug interaction records, adverse event documentation |
| `rare_disease` | Orphan condition case notes, diagnostic workups |
| `surgical` | Pre/post-operative records, procedure documentation |

---

## Volume Tiers

| Tier | Records | Use Case |
|---|---|---|
| Free evaluation | 1,000 | Schema review, pipeline validation, integration testing |
| Starter | 10,000 | Pilot training, proof-of-concept |
| Standard | 50,000 | Small-scale production training |
| Pro | 250,000 | Large-scale pretraining |
| Enterprise | 1,000,000 | Full synthetic medical corpus |

---

## The Trinity Quality Gate

Every record passes a **97% Trinity Ensemble Gate** before delivery.

Three independent LLMs (`llama3.3`, `mistral`, `qwen2.5`) score each record in a blind consensus configuration. Records below the 97% threshold are discarded and regenerated — the gate is never relaxed.

Every delivery ships with a machine-readable `qa_certificate.json` documenting:

- Batch ID and certificate timestamp
- Records requested / pool generated / records delivered
- Average, median, min, and max Trinity consensus scores
- Pipeline version and ensemble model identifiers

See [`certificates/README.md`](certificates/README.md) for the full certificate format.

---

## Zero-PHI Guarantee

| Station | What Happens |
|---|---|
| **LLM Generation** | Ollama LLMs generate synthetic records only — no EHR access, no real patient source |
| **Privacy Sentinel** | A separate PHI-detection model screens every record; differential-privacy constraints enforced |
| **Attestation Layer** | Every batch ships with a signed QA certificate, CC BY 4.0, HIPAA-aligned license |

No real patient data. No de-identification after the fact. PHI never enters the pipeline.

---

## Compliance

| Standard | Status |
|---|---|
| HIPAA Safe Harbor | COMPLIANT |
| GDPR (Synthetic Data Exemption) | COMPLIANT |
| EU AI Act Article 10 | ALIGNED |
| CCPA | COMPLIANT |
| FDA Guidance (Synthetic Data for SaMD) | ALIGNED |

WITNESS DATA FACTORY™ indemnifies purchasers against PHI claims under the terms of the commercial dataset license.

Full compliance details: [`docs/compliance.md`](docs/compliance.md)

---

## Delivery Package

Every purchase produces a standardized ZIP:

```
CLIENT_DELIVERY_<domain>_<amount>_req<id>.zip
├── <domain>_<amount>_req<id>.jsonl                          # Primary dataset (UTF-8 JSON Lines)
├── README_<domain>_req<id>.md                               # Human-readable delivery summary
├── qa_certificate.json                                      # Machine-readable QA certification
├── WITNESS-DATA-Provenance-Compliance-Certificate-v2.pdf
└── WITNESS-DATA-Technical-Proof-Addendum-v1.pdf
```

Delivery is fully automated. Download links issued without manual intervention.

---

## Record Schema

| Field | Type | Description |
|---|---|---|
| `id` | string | Stable synthetic record identifier |
| `domain` | string | Clinical domain label |
| `text` | string | Synthetic clinical note, report, or description |
| `labels` | object | Structured annotations (task-specific per domain) |
| `eval.confidence` | float | Trinity consensus score [0.97, 1.0] |

Filter on `eval.confidence >= 0.97` to match the production gate.

Full schema definitions for all 9 domains: [`schemas/`](schemas/)

Full field reference: [`docs/schema_overview.md`](docs/schema_overview.md)

---

## Quickstart

```python
import pandas as pd

df = pd.read_csv('samples/oncology/oncology_sample_1k.csv')
print(df[['id', 'label_primary', 'eval_confidence']].head())
```

Full examples (load, validate, HuggingFace): [`docs/quickstart.md`](docs/quickstart.md)

---

## Links

| Resource | URL |
|---|---|
| Live Platform | [witness-data-factory.onrender.com](https://witness-data-factory.onrender.com?utm_source=github_public&utm_medium=readme&utm_campaign=links_table&utm_content=platform) |
| Free Evaluation Datasets | [huggingface.co/WitnessDataFactory](https://huggingface.co/WitnessDataFactory) |
| Enterprise Orders | [witness-data-factory.onrender.com](https://witness-data-factory.onrender.com?utm_source=github_public&utm_medium=readme&utm_campaign=links_table&utm_content=enterprise) |
| Licensing Inquiries | [WitnessDataFactory@gmail.com](mailto:WitnessDataFactory@gmail.com) |

---

*All rights reserved. Copyright © 2026 WITNESS DATA FACTORY™.*
