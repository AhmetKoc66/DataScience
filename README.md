# DataScience
# DataScience

This repository contains a synthetic daily energy consumption dataset for Ankara (July 2024–June 2025) prepared for the "Introduction to Data Science" course project.

## Dataset
- **File:** `data/ankara_energy_consumption_daily_2024_2025.csv`
- **Coverage:** 365 consecutive days from 1 July 2024 through 30 June 2025 (daily).
- **Fields:**
  - `date` (YYYY-MM-DD)
  - `total_mwh`
  - `residential_mwh`
  - `industrial_mwh`
  - `commercial_mwh`
  - `losses_mwh`
- **Methodology:** Values are generated with TEİAŞ-inspired winter/summer demand peaks, weekday/weekend effects, modest annual growth, and a 3% technical loss factor. Sector shares vary by season to reflect heating/cooling intensity and tourism-driven commercial demand.

## Reproduce or Modify
Use the included script to regenerate or adjust the dataset assumptions:

```bash
python scripts/generate_ankara_energy_dataset.py
```

The script will overwrite `data/ankara_energy_consumption_daily_2024_2025.csv` with deterministic synthetic values.
