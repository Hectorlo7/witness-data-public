# WITNESS DATA FACTORY™

**Zero-PHI. Production-grade synthetic medical datasets for clinical AI.**

[![Platform](https://img.shields.io/badge/Platform-Live-brightgreen)](https://witness-data-factory.onrender.com)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-WitnessDataFactory-yellow)](https://huggingface.co/WitnessDataFactory)
[![License](https://img.shields.io/badge/License-Commercial-blue)](mailto:WitnessDataFactory@gmail.com)
[![WITNESS GATE](https://img.shields.io/badge/WITNESS%20GATE%20SCORE-%E2%89%A5%200.97-brightgreen)](https://witness-data-factory.onrender.com)

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

> Paid packs (10k → 1M records) sold via **AWS Data Exchange** and delivered via entitlement + presigned download URL.
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

WITNESS DATA FACTORY™ is a deterministic GenAI pipeline that generates, validates, and delivers **production-grade synthetic clinical text datasets** — certified under a **WITNESS GATE SCORE ≥ 0.97** — with zero real patient data ever accessed or stored.

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

> **Requested tier vs delivered rows:** Commercial tiers define the requested batch size and appear in batch IDs, filenames, and package identity. The actual delivered row count is recorded in `records_delivered` in the QA certificate JSON and `final_total` in the Stage 4 quality report. Because automated QA exclusion applies before delivery, the delivered count may be slightly lower than the requested tier size. This is expected and valid behavior.

---

## The WITNESS Quality Gate

Every record passes the **WITNESS GATE** before delivery.

The WITNESS GATE combines:

- deterministic rules, and
- a **two-model ensemble** that scores each record in a blind consensus configuration.

The resulting **WITNESS GATE SCORE** is a continuous quality value in [0, 1]. Records whose WITNESS GATE SCORE falls below `0.97` are discarded and regenerated — the gate is never relaxed.

Every delivery ships with a machine-readable `qa_certificate.json` documenting:

- Batch ID and certificate timestamp
- Records requested / pool generated / records delivered
- Average, median, min, and max WITNESS GATE scores
- Pipeline version and ensemble configuration identifiers

See [`certificates/README.md`](certificates/README.md) for the full QA certificate field reference.

---

## QA Pipeline and Operating Modes

Every production batch is processed through the WITNESS multi-stage validation pipeline before delivery. The pipeline supports two operating modes, recorded in every batch's machine-readable `qa_certificate.json`:

| Mode | `gate_mode` | `witness_gate_status` | Ensemble Active? | ESCALATE Record Handling |
|---|---|---|---|---|
| **Witness Gate** | `witness_gate` | `enabled_for_batch` | Yes — 2-model ensemble | Records failing rules or ensemble threshold are excluded and regenerated |
| **Rules-only** | `rules_only` | `disabled_for_batch` | No — rules only | Records failing rules are excluded; no ensemble scoring is applied |

**In both modes:**

- Only rules PASS and REPAIR records (and, in Witness Gate mode, WITNESS GATE PASS records) are delivered.
- The `qa_certificate.json` delivered with every batch is the **canonical machine-readable source of truth** for `gate_mode`, `witness_gate_status`, `records_delivered`, rejection counts, and all quality metrics.
- The compliance PDFs included in each delivery package are supporting human-readable documents.

---

## Zero-PHI Guarantee

| Station | What Happens |
|---|---|
| **LLM Generation** | Ollama LLMs generate synthetic records only — no EHR access, no real patient source |
| **Privacy Sentinel** | A separate PHI-detection model screens every record; differential-privacy constraints enforced |
| **Attestation Layer** | Every batch ships with a signed QA certificate, manifest, and HIPAA-aligned license |

No real patient data. No de-identification after the fact. PHI never enters the pipeline.

---

## Compliance

| Standard | Status |
|---|---|
| HIPAA Safe Harbor | ✅ COMPLIANT |
| GDPR (Synthetic Data Exemption) | ✅ COMPLIANT |
| EU AI Act Article 10 | ✅ ALIGNED |
| CCPA | ✅ COMPLIANT |
| FDA Guidance (Synthetic Data for SaMD) | ✅ ALIGNED |

WITNESS DATA FACTORY™ indemnifies purchasers against PHI claims under the terms of the commercial dataset license.

Full compliance details: [`docs/compliance.md`](docs/compliance.md)

---

## Delivery Package

Every purchase produces a standardized ZIP:

```
CLIENT_DELIVERY_<domain>_<amount>_req<id>.zip
├── <domain>_<amount>_req<id>.jsonl                          # Primary dataset (UTF-8 JSON Lines)
├── README_<domain>_req<id>.md                               # Human-readable delivery summary
├── qa_certificate_<domain>_req<id>.json                     # Machine-readable QA certification (canonical batch record)
├── delivery_manifest_<domain>_req<id>.json                  # File-level hashes and audit trail
├── WITNESS-DATA-Provenance-Compliance-Certificate-v2.pdf
├── WITNESS-DATA-Technical-Proof-Addendum-v1.pdf
└── WITNESS-DATA-License-Compliance-Framework-v1.pdf
```

The `qa_certificate.json` and `delivery_manifest.json` are the **authoritative machine-readable records** for the batch. The three PDFs are supporting human-readable compliance and audit documents.

Delivery is fully automated. Download links issued without manual intervention.

---

## Record Schema

| Field | Type | Description |
|---|---|---|
| `id` | string | Stable synthetic record identifier |
| `domain` | string | Clinical domain label |
| `text` | string | Synthetic clinical note, report, or description |
| `labels` | object | Structured annotations (task-specific per domain) |
| `eval.confidence` | float | Rules-based QA confidence score; in Witness Gate mode, reflects the WITNESS GATE SCORE |

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
| Enterprise Orders (AWS Data Exchange) | [witness-data-factory.onrender.com](https://witness-data-factory.onrender.com?utm_source=github_public&utm_medium=readme&utm_campaign=links_table&utm_content=enterprise) |
| Licensing Inquiries | [WitnessDataFactory@gmail.com](mailto:WitnessDataFactory@gmail.com) |

---

*All rights reserved. Copyright © 2026 WITNESS DATA FACTORY™.*
