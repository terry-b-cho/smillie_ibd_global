# Smillie IBD Global Research Project

A research project analyzing DNA methylation differences between inflammatory bowel disease (IBD) patients and healthy controls across US and Indian cohorts.

## Project Structure

```
smillie_ibd_global/
├── data/
│   └── methylation/
│       ├── CDSA_metadata.csv            # Clinical and demographic metadata
│       ├── epiSampleID_2_subjectID.txt  # Sample ID mapping file
│       ├── US_epic_beta.csv             # US cohort EPIC array beta values
│       ├── US_epic2_beta.csv            # US cohort EPICv2 array beta values
│       ├── India_epic2_beta.csv         # India cohort EPICv2 array beta values
│       ├── EPIC_annotation_table.csv    # EPIC array probe annotations
│       └── EPICv2_annotation_table.csv  # EPICv2 array probe annotations
├── notebook/
│   └── processing.ipynb                 # Main analysis notebook
└── env/                                 # Virtual environment (excluded from repo)
```

## Analysis Overview

The project performs differential methylation analysis comparing IBD patients to healthy controls using:

- **US Cohort**: EPIC and EPICv2 methylation arrays
- **India Cohort**: EPICv2 methylation arrays  
- **Statistical Testing**: Rank-sum tests for differential methylation
- **Visualization**: Manhattan plots showing genome-wide results
- **Annotation**: Gene mapping and functional annotation of significant sites

## Key Data Files

- **Beta Values**: Processed methylation data (proportion of methylated cytosines per CpG site)
- **Metadata**: Sample clinical information and disease status
- **Sample Mapping**: Links epigenetic sample IDs to subject identifiers
- **Annotations**: Genomic coordinates and gene information for methylation probes

## Requirements

- Python 3.7+
- Jupyter Notebook
- pandas, numpy, scipy
- matplotlib, seaborn
- tqdm for progress tracking

## Usage

1. Clone repository and create virtual environment
2. Install dependencies: `pip install -r requirements.txt`
3. Ensure data files are in `data/methylation/` directory
4. Run `notebook/processing.ipynb` for complete analysis pipeline

## Data Access

The data directory is excluded from this repository for privacy protection. Methylation data contains sensitive information and requires appropriate ethical approvals for access.

## License

Modified MIT License with restrictions for academic and non-commercial use only. See LICENSE file for complete terms.

## Citation

[Citation information to be added upon publication] 