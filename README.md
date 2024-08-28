# CUHK-2024Summer-Mentorship

## Meta Information
This github repository contains information about codes, reports, and datasets regarding the mentotship project and job ads extraction project.

### Related Literature
- [Diversifying the Professoriate by Hofstra et al.](https://journals.sagepub.com/doi/full/10.1177/23780231221085118)
- [The academic Great Gatsby Curve by Sun et al.](https://royalsocietypublishing.org/doi/10.1098/rsif.2024.0173)
- [Slow convergence: Career impediments to interdisciplinary biomedical research by Berkes et al.](https://www.pnas.org/doi/full/10.1073/pnas.2402646121)


## Mentorship Project
- The original dataset: [The Original "Mentorship Dataset"](https://zenodo.org/records/4917086)
- The original dataset paper: [A dataset of mentorship in bioscience with semantic and demographic estimations](https://www.nature.com/articles/s41597-022-01578-x)
- Our processed dataset: [The HuggingFace Dataset](https://huggingface.co/datasets/Matthewfung/24Summer_RA/tree/main)

### Files and Folders
- ***The HuggingFace Dataset/***: The HuggingFace dataset contains all original mentorship data as well as our expanded data. Details are written in the HuggingFace dataset page. The dataset is set as public so it can be easily accessed via Python IDEs like Google Colab.

- ***Analysis/***: This folder contains data analysis regarding within person/field similarities (or distances as they measures how distant two vectors are), topic choices, pairings, etc.
    - ***Field_Typicality&Citation.ipynb***: This notebook measures the within field similarity and ciation counts of researchers.
    - ***OLS.ipynb***: This notebook runs simple linear regression on the final dataset (i.e., the final expanded dataset).
    - ***WithinPerson&T-tests.ipynb***: This notebook runs within person analysis and topic choices analysis using the original mentorship dateset.

- ***OpenAlex/***: This folder contains scripts for mapping MAGIDs in mentorship dataset to OpenAlex project.
    - ***AWS_Mapping.ipynb***: This notebook contains codes that downloads a snapshot dateset of OpenAlex and extract relevant data using MAGIDs in mentorship dataset.
    - ***Institution_H_Index.ipynb***: This notebook deals with inconsistancies in H_index json formatted data of OpenAlex.

## Job Ads Extraction Project

### Files and Folders
- ***Job Ads Extraction/***: This folder contains scripts for extracting major requirements in job Ads.
    - ***Job_Ads_Extraction.ipynb***: This notebook compares the performances of different Large Language Models on extracting information related to major requirements .
