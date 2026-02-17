
# Introduction

  

This repository contains code and data for my article "[Connecting Patients to Drug Trials: Federating OMOP CDM and Ducklake Knowledge Graph](https://medium.com/@dgg32/graph-visualization-for-duckpgq-e6a551d11b94)".



# Prerequisite

Docker

MotherDuck account

DuckDB

Python


# Run

1. Run OMOP CDM on Broadsea Docker

Follow the commands in commands.txt to run OMOP CDM on Broadsea Docker.

2. Prepare the data

Use trial_condition_to_cui.ipynb to extract unique medical conditions from trials_umls.tsv and annotate them with UMLS CUI

Use add_condition_cui_to_trials.ipynb to add the medical condition CUI to trials_umls.tsv

Use convert_moa_to_cui.ipynb to map the MOA ID to UMLS CUI.

Use source_to_concept_map.ipynb to add condition and drug mapping to the source_to_concept_map table. It lays out the mapping between OMOP and UMLS.


3. MotherDuck

Use ducklake_setup.ipynb to set up Ducklake on MotherDuck

Use query_ducklake_omop.ipynb to query Ducklake and OMOP


## Authors



*  **Sixing Huang** - *Concept and Coding*

  

  

## License

  

  

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
