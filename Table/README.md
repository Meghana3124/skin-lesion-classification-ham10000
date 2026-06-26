# Dataset Preview

## Overview

The table below shows the first five records of the **HAM10000 metadata dataset**, which contains information about each dermoscopic skin lesion image used in this project.

This metadata is used to associate each image with its corresponding diagnosis and patient information before preprocessing and model training.

---

## Table Description

| Column | Description |
|--------|-------------|
| **lesion_id** | Unique identifier assigned to each skin lesion. Multiple images may belong to the same lesion. |
| **image_id** | Unique identifier for each dermoscopic image. Used to locate the image file in the dataset. |
| **dx** | Diagnostic class (skin lesion type). Examples include *akiec, bcc, bkl, df, mel, nv,* and *vasc*. |
| **dx_type** | Method used to confirm the diagnosis, such as histopathology (`histo`). |
| **age** | Age of the patient in years. |
| **sex** | Gender of the patient (Male or Female). |
| **localization** | Anatomical location of the skin lesion (e.g., scalp, ear, back, face, trunk). |

---

## Sample Dataset

| lesion_id | image_id | dx | dx_type | age | sex | localization |
|-----------|----------|----|---------|-----|------|--------------|
| HAM_0000118 | ISIC_0027419 | bkl | histo | 80 | Male | Scalp |
| HAM_0000118 | ISIC_0025030 | bkl | histo | 80 | Male | Scalp |
| HAM_0002730 | ISIC_0026769 | bkl | histo | 80 | Male | Scalp |
| HAM_0002730 | ISIC_0025661 | bkl | histo | 80 | Male | Scalp |
| HAM_0001466 | ISIC_0031633 | bkl | histo | 75 | Male | Ear |

---

## Purpose

This metadata table is essential for:

- Linking image files with their diagnostic labels.
- Performing data preprocessing and label encoding.
- Analyzing patient demographics.
- Splitting the dataset into training, validation, and testing subsets.
- Supporting supervised learning for skin lesion classification.

---

## Notes

- Each **image_id** corresponds to one dermoscopic image.
- A single **lesion_id** may have multiple associated images captured from different angles.
- The metadata is stored in the file **HAM10000_metadata.csv** and is used throughout the deep learning pipeline.
