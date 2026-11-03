# ToxiScope Predict and Results demo data

This public repository hosts versioned data bundles used by the ToxiScope Streamlit demo. It contains no application source code. The release `predict-results-v2` contains one asset: `toxiscope-core-v2.zip` (19,467,752 bytes; SHA-256 `5c356e7ad8086069162cebfe9c43f26dc4774e231ce75ce5cfb4db40102ec877`).

## Contents and reuse

The archive includes RDKit Morgan fingerprints and audited molecule/assay rows derived from the DeepChem/MoleculeNet Tox21 distribution, a ToxiScope-fitted random forest, and the attribution notice. It excludes PubMed abstracts, literature summaries, search indexes and BiomedBERT. The underlying federal Tox21 assay facts are described as public domain in an [NCATS presentation hosted by NIEHS](https://ntp.niehs.nih.gov/sites/default/files/iccvam/meetings/iccvam-forum-2020/ppt/13-ncats-simeonov-508.pdf) (May 21, 2020, pages 4 and 7). See the [official challenge data](https://tripod.nih.gov/tox21/challenge/data.jsp) and [NIEHS Tox21 program](https://www.niehs.nih.gov/research/programs/tox21).

The local source is the historical DeepChem/MoleculeNet CSV snapshot (`https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/tox21.csv.gz`; SHA-256 `45d09792492ce049039dd24aa27b07fc79ce20c573187d4d90bcd178c0c0d360`). The [DeepChem loader](https://github.com/deepchem/deepchem/blob/master/deepchem/molnet/load_function/tox21_datasets.py) documents the mirror and columns. This is curated MoleculeNet data, not the complete original challenge release. No separate machine-readable license accompanies the mirror; this repository does not infer a dataset-wide MIT license from DeepChem software or declare the mirror CC0. Preserve `NOTICE.txt` when redistributing the archive. No agency or DeepChem endorsement is implied. These in-vitro results are not a human toxicity or clinical safety assessment.

Only publish the versioned demo archive and its accompanying notice. Do not add literature or research artifacts here.
