## Data Analysis and Data Pipeline Through R Handling PSID Data
#### psid-panel

This repository supports a longitudinal data-building project for academic research at Hope College, supervised by Dr. Silveus and used within the Frost Research Center.
The code constructs a clean, analysis-ready PSID family–year panel by automating the reading and alignment of raw PSID fixed-width data files across survey waves.
It is designed for reproducibility and extension, researchers or students can add new years or variables simply by updating the crosswalk CSVs, rather than manually re-parsing the fixed-width files.

Build a longitudinal, family-year panel from PSID fixed-width text files (FAM####ER.txt) using the official layout dictionaries (.sps or .do).
The pipeline reads each wave, renames variables via simple CSV crosswalks, and writes a tidy panel to Parquet for fast downstream work.

Result: one row per family per interview year, with a stable set of columns across waves.


#### Requirements

R ≥ 4.2

Packages: readr, dplyr, stringr, tibble, purrr, fs, glue, here, arrow

Install once

#### License
Code in this repository is released under an MIT-style license. PSID data files are not included and are governed by PSID’s own licenses/terms.


### Contact
Maintainer: Sam Buck (Hope College)  
Email: samuellorenbuck@gmail.com  
For questions about the PSID variables, structure, or extending the panel build scripts, feel free to reach out.
