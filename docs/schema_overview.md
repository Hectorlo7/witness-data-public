# Schema Overview — All 9 Domains

Every WITNESS DATA FACTORY™ record follows a consistent base schema with domain-specific label extensions.

## Base Schema (All Domains)

| Field | Type | Description |
|---|---|---|
| `id` | string | Stable synthetic record ID (e.g., `ONC-000001`) |
| `domain` | string | Clinical domain label |
| `text` | string | Synthetic clinical note, report, or description |
| `labels` | object | Domain-specific structured annotations |
| `eval.confidence` | float | Trinity consensus score [0.97–1.0] |
| `eval.model_version` | string | Pipeline version that generated the record |

## Domain-Specific Label Fields

| Domain | Key Label Fields |
|---|---|
| `oncology` | `primary_diagnosis`, `stage`, `histology`, `icd10` |
| `cardiology` | `primary_diagnosis`, `icd10`, `severity` |
| `neurology` | `primary_diagnosis`, `icd10`, `severity` |
| `pathology` | `primary_diagnosis`, `icd10`, `specimen_type` |
| `radiology` | `primary_finding`, `modality`, `impression` |
| `endocrinology` | `primary_diagnosis`, `icd10`, `severity` |
| `pharmacology` | `event_type`, `icd10`, `severity` |
| `rare_disease` | `primary_diagnosis`, `icd10`, `orphanet_code` |
| `surgical` | `primary_procedure`, `icd10`, `phase` |

## Quality Filter

All delivered records meet `eval.confidence >= 0.97`.

To reproduce the production gate filter:

```python
filtered = [r for r in records if r['eval']['confidence'] >= 0.97]
```

Full JSON schemas for each domain are in the `/schemas/` directory.
