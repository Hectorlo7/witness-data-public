# Quickstart Guide

## Load a Sample in Python

```python
import pandas as pd

# Load a WITNESS DATA FACTORY sample CSV
df = pd.read_csv('samples/oncology/oncology_sample_1k.csv')

print(df.shape)          # (10, 7)
print(df.columns.tolist())
print(df['text'].iloc[0])
```

## Load a Full Paid Delivery (JSONL)

```python
import json

records = []
with open('oncology_50000_req142.jsonl', 'r') as f:
    for line in f:
        records.append(json.loads(line))

# Filter to highest-confidence records
top = [r for r in records if r['eval']['confidence'] >= 0.985]
print(f'{len(top)} records above 0.985 threshold')
```

## Validate Against Schema

```python
import json
import jsonschema

with open('schemas/oncology_schema.json') as f:
    schema = json.load(f)

# Validate a record
record = {
    "id": "ONC-000001",
    "domain": "oncology",
    "text": "Patient is a 58-year-old female...",
    "labels": {"primary_diagnosis": "NSCLC", "stage": "IIIA"},
    "eval": {"confidence": 0.991, "model_version": "trinity-v2.4.1"}
}

jsonschema.validate(record, schema)
print("Record is valid.")
```

## Use with HuggingFace Datasets

```python
from datasets import load_dataset

ds = load_dataset('WitnessDataFactory/oncology-synthetic-clinical-notes')
print(ds)
```

## Order Paid Packs

Visit the live checkout:

```
https://witness-checkout.onrender.com/checkout?domain=oncology&tier=50K
```

Replace `domain` with any of the 9 domains and `tier` with `10K`, `50K`, `250K`, or `1M`.

Delivery is automated. Download link issued within minutes of payment.
