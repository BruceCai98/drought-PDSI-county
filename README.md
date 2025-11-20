# drought-PDSI-county
County-level Monthly PDSI (1990–2024) for the Contiguous United States, computed from METDATA/THREDDS Palmer Drought Severity Index. Python pipeline for downloading, processing, spatial clipping, and aggregating daily PDSI into county-level monthly panel data.
# County-Level Monthly PDSI (1990–2024)

This repository provides a full Python workflow for downloading, processing, 
and aggregating **daily Palmer Drought Severity Index (PDSI)** data from the 
Northwest Knowledge Network (NKN) THREDDS server into **county-level monthly 
drought panel data** for the contiguous United States (CONUS) from **1990 to 2024**.

The final output is a tidy panel dataset:

GEOID | time | pdsi
01001 | 1990-01-01 | -1.23
01001 | 1990-02-01 | -0.54
...


This dataset is suitable for use in:
- Econometric panel regressions  
- Agricultural economics research  
- Drought impact studies  
- Environmental / climate statistics  
- County-level socio-environmental analysis  

---

## Data Source

We use the **Palmer Drought Severity Index (PDSI)** from:

**NKN / METDATA / REACCH aggregated products**  
OPeNDAP URL:

https://thredds.northwestknowledge.net/thredds/dodsC/agg_met_pdsi_1979_CurrentYear_CONUS.nc


This dataset provides **daily gridded PDSI** for CONUS from 1979–current year, with:

- Spatial resolution: ~4 km  
- Coordinates: `lat`, `lon`
- Time dimension: `day`
- Key variable used:  
  `daily_mean_palmer_drought_severity_index`

If you use the county-level processed dataset created by this repository, please cite:

Cai (2025). County-level Monthly PDSI (1990–2024). GitHub Repository.
URL: https://github.com/BruceCai98/drought-PDSI-county
---
---
## Contact

For questions, feel free to open an issue or contact:
Zhangchi (Bruce) Cai
UW–Madison, Agricultural & Applied Economics
zcai98@wisc.edu


