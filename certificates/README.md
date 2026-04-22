# QA Certificates

Every paid delivery from WITNESS DATA FACTORY™ includes a `qa_certificate.json` alongside the dataset.

## Certificate Format

```json
{
  "certificate_id": "CERT-2026-ONC-00142",
  "issued_at": "2026-04-22T02:00:00Z",
  "domain": "oncology",
  "tier": "50K",
  "batch_id": "BATCH-ONC-20260422-00142",
  "records_requested": 50000,
  "records_generated": 58312,
  "records_delivered": 50000,
  "trinity_gate_threshold": 0.97,
  "trinity_scores": {
    "mean": 0.984,
    "median": 0.986,
    "min": 0.971,
    "max": 0.998
  },
  "pipeline_version": "trinity-v2.4.1",
  "ensemble_models": ["llama3.3", "mistral", "qwen2.5"],
  "license": "CC BY 4.0 — Commercial Dataset License",
  "phi_attestation": "ZERO_PHI — no real patient data accessed or stored",
  "hipaa_status": "HIPAA Safe Harbor Compliant"
}
```

Certificates are machine-readable and audit-ready. Every batch ID is traceable to the generation pipeline.
