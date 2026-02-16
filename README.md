# portal-vein-diameter
Code for portal vein diameter automated measurement manuscript

This repository contains the statistical analysis code used in:

Hartmann K*, Beeche C, Judy R, DePietro DM, Witschey WR, Duda J, Gee J, Gade T, Penn Medicine Biobank, Levin MG, Damrauer SM.

Portal Vein Diameter on Routine Clinical CT: Establishing Normals and Disease Associations.  
Submitted to *Radiology*, 2026.

*Corresponding author

## Contact

Katherine Hartmann, MD, PhD  
Department of Radiology  
University of Pennsylvania  
Email: katherine.hartmann@pennmedicine.upenn.edu

---

## Overview

This repository includes code to:

- Compare automated vs manual portal vein diameter measurements
- Perform Bland–Altman agreement analysis
- Compute intraclass correlation coefficients (ICC)
- Conduct univariable and multivariable regression analyses
- Perform time-to-event (Cox proportional hazards) analyses
- Generate publication-quality figures and forest plots

All analyses were conducted using R.

---

## Data Availability

Due to institutional review board and data use agreement restrictions, raw participant-level data cannot be shared.

The scripts assume access to a de-identified dataset structured as described below. Researchers interested in accessing the underlying data should contact the corresponding author according to institutional policies.

---

## Expected Data Structure

The analysis scripts assume a dataset containing the following types of variables:

- De-identified participant identifier
- Portal vein diameter (automated measurement)
- Manual measurement (subset)
- Demographics (age, sex, race)
- Anthropometrics (BMI, height)
- Exam characteristics (exam type, site)
- Clinical outcomes (liver disease, portal hypertension, ascites, varices)
- Time-to-event variables where applicable

Variable names may need to be adapted to match local datasets.

---

## Software Environment

Required R packages include:

- tidyverse
- lme4
- lmerTest
- survival
- broom
- sandwich
- lmtest
- ggplot2
- forestplot
- irr
- data.table (if applicable)

