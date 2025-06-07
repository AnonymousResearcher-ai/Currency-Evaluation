# ICDM 2025 Anonymous Submission

This repository contains the full implementation and evaluation code for an ICDM 2025 paper submission focused on currency evaluation through classification, usability assessment, and counterfeit detection.

## Overview

The project provides a unified framework for:

* Denomination classification using lightweight and pre-trained CNNs
* Damage quantification using binary, chromatic, and symbolic features
* Counterfeit detection through structural feature matching

All modules are implemented in Jupyter notebooks and organized for reproducibility.

## Repository Structure

```
├── data/                      # Torn Results
├── data_torn/                 # Torn note samples for usability analysis
├── standard_notes/           # Reference templates for alignment
├── 0_dataset_preparation.ipynb           # Initial dataset cleaning and deduplication
├── 1_data_split_and_augmentation.ipynb   # Split and augment datasets
├── 2_classification_all_datasets.ipynb   # Run classification across 4 CNN models
├── 3_customCNN_all_datasets.ipynb        # Train and evaluate a custom lightweight CNN
├── 4_usability_analysis.ipynb            # Damage assessment and CCDS score generation
├── 5_fake_currency_detection.ipynb       # Counterfeit detection using template matching
├── LICENSE
├── README.md
```

## Datasets
Dataset details are provided in the paper.

## Environment

* Python 3.8+
* PyTorch
* OpenCV
* scikit-learn, seaborn, matplotlib

You can recreate the virtual environment using:

```bash
python -m venv dmp
source dmp/bin/activate
```

## Usage

Each numbered notebook represents a pipeline stage:

* Start with `0_dataset_preparation.ipynb` to clean and deduplicate.
* Continue through `1_data_split_and_augmentation.ipynb` and train using `2_` and `3_` series.
* Run `4_` for damage quantification and `5_` for counterfeit detection.

## Notes

* All image-based data used are public or synthetic.
* This repository has been anonymized for double-blind review.
* All figures, metrics, and scores reported in the paper can be regenerated from the notebooks.

## License

Released for academic, non-commercial research use only.

---

For questions, please reach out after the review period.
