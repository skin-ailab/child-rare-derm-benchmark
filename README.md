# Rare Pediatric Dermatology Benchmark Dataset

[![License](https://img.shields.io/badge/License-CC_BY_NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.xxxxxxx.svg)](https://doi.org/10.5281/zenodo.xxxxxxx)

A curated collection of clinically validated cases for rare childhood dermatological conditions, designed to support research in:
- Rare disease diagnosis
- Dermatological pattern recognition
- Clinical decision support systems
- Medical education

## Dataset Overview

**Structure**:  
```json
{
  "title": "Case Title",
  "history_and_symptoms": "Clinical presentation details",
  "examination": "Diagnostic procedures & findings",
  "treatment": "Therapeutic interventions",
  "diagnosis": "Final diagnosis & clinical significance"
}
```

## Key Features
- 28 validated clinical cases (initial release)
- Standardized JSON format for ML compatibility
- De-identified patient information

## Example Cases

### Case 1: Juvenile Vulvar Pemphigoid
```json
{
  "title": "The diagnostic difficulties of juvenile vulvar pemphigoid",
  "history_and_symptoms": "8-year-old girl with recurrent vulvar blisters...",
  "examination": "Subepidermal cleft with eosinophils...",
  "treatment": "Topical clobetasol followed by oral steroids...",
  "diagnosis": "Demonstrates diagnostic challenges of childhood bullous pemphigoid..."
}
```

### Case 2: Atypical Tuberculid Coexistence
```json
{
  "title": "Co-existence of atypical tuberculid with lupus vulgaris",
  "history_and_symptoms": "11-year-old Kuwaiti girl with 6-year history...",
  "examination": "Epithelioid cell granulomas with Langhans giant cells...",
  "treatment": "Anti-tuberculosis therapy regimen...",
  "diagnosis": "Rare combination of cutaneous tuberculosis manifestations..."
}
```

## Usage
```bash
git clone https://github.com/skin-ailab/rare-peds-derm-benchmark.git
```

```python
import json

with open('cases.json') as f:
    cases = json.load(f)
    
print(f"Available cases: {len(cases)}")
print(f"First case diagnosis: {cases[0]['diagnosis']}")
```

## Contribution Guidelines
1. Fork the repository
2. Add new cases following our [JSON schema](schema.json)
3. Submit pull request with:
   - Complete clinical documentation
   - De-identified patient data
   - Institutional review board approval evidence

## License  
CC BY-NC 4.0: Permits non-commercial use with proper attribution.
 



