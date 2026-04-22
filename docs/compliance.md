# Compliance & Licensing

## Zero-PHI Architecture

WITNESS DATA FACTORY™ generates synthetic clinical records entirely from LLM inference. No real patient data is accessed, processed, stored, or referenced at any point in the pipeline.

| Station | Mechanism |
|---|---|
| Generation | Ollama LLMs (llama3.3, mistral, qwen2.5) produce synthetic text only |
| PHI Sentinel | Separate PHI-detection model screens every record pre-delivery |
| Attestation | Signed `qa_certificate.json` shipped with every batch |

## Compliance Status

| Standard | Status | Notes |
|---|---|---|
| HIPAA Safe Harbor | ✅ COMPLIANT | Synthetic data, no real PHI |
| GDPR | ✅ COMPLIANT | Synthetic data exemption applies |
| EU AI Act Art. 10 | ✅ ALIGNED | High-quality training data requirements |
| CCPA | ✅ COMPLIANT | No personal information collected or processed |
| FDA SaMD Guidance | ✅ ALIGNED | Synthetic data for Software as a Medical Device |

## License

All datasets are delivered under a **CC BY 4.0 Commercial Dataset License**.

Purchasers are indemnified against PHI claims under the terms of the commercial dataset license.

## Contact

Licensing inquiries: WitnessDataFactory@gmail.com
