# 📊 Educator EdTech Usage (Arabic Dataset)

## Overview

This project analyzes the use and knowledge of digital and AI-based tools among educators in Arabic-speaking contexts. Based on a structured survey of teachers across various experience levels and school types, the study identifies trends, gaps, and influencing factors related to the integration of educational technologies in teaching practices.

The dataset includes 39 variables representing self-reported **knowledge** and **actual use** of tools like LMSs, digital assessments, AI content generation, and more. The analysis highlights gender-specific trends, experience-based differences, and the overall readiness of educators to adopt emerging technologies.

---

## 🧾 Dataset Features

- **Knowledge & Use scores** (Likert scale 1–5) for:
  - LMS platforms
  - AI-based lesson planning
  - Digital assessments
  - Collaboration & content tools
- **Demographic data**:
  - Gender, Age group, Years of experience, Specialization
- **Arabic-language labels** requiring reshaping and BiDi rendering

---

## 🔍 Data Processing

- **Text Preparation**: Used `arabic-reshaper` and `python-bidi` to reshape Arabic labels for proper right-to-left rendering in visual outputs.
- **Column Segmentation**: The wide dataset with 39 columns was split into 4 horizontal segments, each saved as a standalone image for better readability.
- **Descriptive Statistics**: Means and standard deviations were calculated for each tool’s knowledge and use scores.
- **Statistical Tests Applied**:
  - **Shapiro-Wilk Test**: Tested for normality
  - **Mann-Whitney U Test**: Gender-based comparisons
  - **Kruskal-Wallis Test + Dunn’s Post-hoc**: Experience group comparisons
  - **Spearman Correlation**: Relationship between knowledge and use

---

## 📊 Visuals

All output visualizations are stored in the `visuals/` directory, including:

- `columns_segment_1.png` to `columns_segment_4.png` – Segmented dataset table images
- `knowledge_use_means.png` – Average scores and standard deviations
- `gender_boxplots.png` – Knowledge/use comparison between genders
- `experience_boxplots.png` – Knowledge/use by experience group
- `correlation_heatmap.png` – Spearman correlation heatmap

---

## 🧪 Technologies Used

- **Python 3.x**
- **Key Libraries**:
  - `pandas` – Data loading and manipulation
  - `numpy` – Numerical computations
  - `matplotlib` / `seaborn` – Data visualization
  - `scipy` – Statistical analysis
  - `arabic-reshaper` + `python-bidi` – Arabic text formatting for RTL tables
