# Pan-Metabolomics Repository Mapping of the Carnitine Landscape

This repository contains all data and scripts associated with the manuscript **"Pan-Metabolomics Repository Mapping of the Carnitine Landscape"**.

---

## Repository Contents

### `Figures/`
This folder contains the scripts used to generate all figures and supplementary figures in the manuscript, along with the input tables and source data for each of them.

### `Data_processing_MZmine/`
This folder contains all MZmine batch files used to pre-process the metabolomics data discussed in this manuscript. 

### `Supplementary Tables/`
This folder contains all supplementary tables referenced in the manuscript, provided as .csv files.

### `GNPS-CANDIDATE-CARNITINES-MASSQL.zip`
Carnitine spectral library created for this work. This library consists of 34,222 representative MS/MS spectra from Falcon-clustered spectra of public data on GNPS/MassIVE, MetaboLights, and Metabolomics Workbench, recovered using MassQL queries designed for carnitines. This library contains MS/MS spectra of 2,857 potential modifications that carnitines can undergo, described as delta masses. Molecular formulae for the delta masses are provided as predicted by two *in silico* tools, BUDDY and SIRIUS, along with putative explanations when available.

> This library is available in the GNPS environment through the following link:
> https://gnps.ucsd.edu/ProteoSAFe/gnpslibrary.jsp?library=GNPS-CANDIDATE-CARNITINES-MASSQL

---

## MassQL Query

The following query was used to recover potential carnitine MS/MS spectra from public metabolomics repositories:
```
QUERY scaninfo(MS2DATA) WHERE
MS2PROD=60.0808:TOLERANCEPPM=20:INTENSITYPERCENT=1 AND
MS2PROD=85.0284:TOLERANCEPPM=20:INTENSITYPERCENT=50 AND
MS2PROD=144.1019:TOLERANCEPPM=20:INTENSITYPERCENT=1
```

All queries were executed using the GNPS2 MassQL workflow, and the results can be accessed through the following links:

- **MetaboLights:** https://gnps2.org/status?task=a61b20c5251242afb60ff193146bd1d0
- **Metabolomics Workbench:** https://gnps2.org/status?task=268a473d58644fddaafdcd6f03ad94cd
- **GNPS/MassIVE (Orbitrap collection):** https://gnps2.org/status?task=25a8a3ff61e94fcaad99faa6a556faa5
- **GNPS/MassIVE (QE collection):** https://gnps2.org/status?task=e9013a4b1e94438f97e501122239e71c
- **GNPS/MassIVE (QToF collection):** https://gnps2.org/status?task=b27657fb7c854fdd9106bcd6ea446890

---

## Citation

> *(to be added upon publication)*

---

## Contact

For more information and questions regarding these scripts please reach out to hmannochiorusso@health.ucsd.edu and fpatrick@health.ucsd.edu
