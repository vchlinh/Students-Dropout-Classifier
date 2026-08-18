# Student Academic Success & Dropout Prediction

A machine learning project analyzing the factors that influence undergraduate academic outcomes, with a focus on identifying students at risk of dropping out.

## Overview

Using a dataset of **4,424 undergraduate students** from the UCI Machine Learning Repository, this project investigates whether demographic, socioeconomic, and early-college academic information can predict three student outcomes: **Dropout, Enrolled, and Graduate**.

**Research question:**  
> Which factors are most predictive of student academic outcomes, particularly dropout risk?

## Approach

- Performed data cleaning, categorical encoding, and **feature engineering** in R
- Conducted exploratory data analysis and feature selection
- Built and compared **Random Forest** and **Gradient Boosted Trees using XGBoost**
- Fine-tuned model hyperparameters using cross-validation
- Generated **feature importance plots** to identify the strongest predictors

## Results

Early-college academic performance emerged as the strongest predictor of student outcomes.

Key predictors included:

- First-year curricular units **approved**
- First-year **grades**
- Curricular units **enrolled**
- Course/major
- Admission grade
- Tuition payment status
- Parents' occupations
- Student debt status

| Model | Cross-Validated Accuracy |
|---|---:|
| Random Forest | **77.48%** |
| XGBoost | **77.82%** |

By incorporating **early-college performance features**, the models achieved approximately **5% higher out-of-sample accuracy than prior studies** that relied primarily on pre-college and demographic information.

## Tech Stack

**R** · `tidyverse` · `ggplot2` · `tidymodels` · `randomForest` · `xgboost` · `vip`

## Dataset

**UCI Machine Learning Repository — Predict Students' Dropout and Academic Success**

The dataset contains demographic, socioeconomic, and academic information from students at the Polytechnic Institute of Portalegre, Portugal.

## Key Takeaway

The analysis suggests that **early academic performance is a substantially stronger signal of student outcomes than many demographic or socioeconomic characteristics**, highlighting the potential for early identification and intervention for students at risk of dropping out.

## Authors

**Duc Nguyen & Linh Vu** · Grinnell College
