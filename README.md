# Hospital Admissions Analysis in Python

## 1. Project Overview

This project analyses a small dataset of **hospital admissions** using Python and basic data structures.

Each record describes a single hospital stay (ricovero) for a patient, including:

- patient identifiers and region of residence;
- admission and discharge dates;
- presence of **cardiac** and **respiratory** comorbidities;
- COVID-19 swab result (positive/negative);
- type of admission (standard vs specialist);
- clinical diagnosis. :contentReference[oaicite:0]{index=0}  

The main goals of the project are:

1. **Model hospital admissions** with an object-oriented approach (`Ricovero` class).
2. **Compute key indicators** such as:
   - length of stay for each patient,
   - total cost of the healthcare service per admission,
   - distribution of admissions by region and time period,
   - median length of stay for specific time windows,
   - percentage of patients with cardiopulmonary comorbidities.
3. **Perform simple data analysis** using both pure Python and the `pandas` library to extract aggregated information from the dataset.   

---

## 2. Dataset

The main input file is:

- `PAZIENTI.txt` – raw admissions data, one record per line, colon-separated.

Each line has the following structure:

```text
ID_RICOVERO:COD_FISCALE:NOME:COGNOME:REGIONE:DATA_INIZIO:DATA_FINE:PATOLOGIE_CARDIACHE:PATOLOGIE_RESPIRATORIE:ESITO_COVID:DIAGNOSI

