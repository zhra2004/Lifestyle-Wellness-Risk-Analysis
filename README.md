# Lifestyle & Wellness Risk Analysis

An exploratory data analysis and interactive dashboard project that examines lifestyle patterns and their relationship with health risk classifications using Python and Power BI.

## 1. Project Overview

Lifestyle choices play an important role in overall health and well-being. Understanding how individual lifestyle factors contribute to cumulative risk profiles can help identify population groups that may require greater attention to preventive health initiatives.

This project analyzes lifestyle and demographic data to explore patterns associated with different health risk levels. A weighted rule-based scoring approach is developed using four lifestyle factors: sleep quality, physical activity, dietary habits, and smoking status.

The analysis is presented through an interactive Power BI dashboard to provide insights into population risk distributions and lifestyle patterns across different demographic groups.

## 2. Problem Statement

How do individual lifestyle factors and their cumulative effects relate to health risk levels, and how can rule-based risk profiling help identify population groups with higher vulnerability to health risks?

## 3. Project Objectives

- Examine the distribution of health risk classifications across the population.
- Analyze lifestyle patterns associated with different risk categories.
- Explore health risk distributions across demographic and socioeconomic groups.
- Develop a weighted rule-based scoring system to classify individuals based on cumulative lifestyle risk factors.
- Identify population groups that may benefit from targeted preventive health initiatives.

## 4. Dataset Overview

The dataset contains demographic, socioeconomic, lifestyle, and health-related information.

| Dataset Attribute | Description |
|---|---|
| Total Records | 413,768 |
| Total Features | 16 |
| Categorical Features | 13 |
| Numerical Features | 3 |
| Missing Values | 0 |

The dataset includes variables related to age, employment, lifestyle habits, and health conditions.

**Dataset Source:** [Insert original dataset source and URL]

## 5. Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data exploration, cleaning, and preparation |
| Pandas | Data manipulation and preprocessing |
| Power BI | Interactive dashboard development |
| DAX | Measures and dashboard calculations |
| Microsoft Excel | Supporting data inspection and validation |

## 6. Data Preparation

The data preparation process involved the following steps:

1. **Data Inspection:** Examined dataset structure, data types, and variable characteristics.
2. **Data Cleaning:** Checked data consistency and missing values.
3. **Feature Selection:** Selected relevant demographic, socioeconomic, lifestyle, and health-related variables for analysis.
4. **Feature Engineering:** Created additional variables, including Risk Score and Risk Status, using the selected lifestyle factors.
5. **Data Transformation:** Prepared the dataset for further analysis and dashboard development.

## 7. Methodology: Weighted Rule-Based Risk Profiling

This project applies a weighted rule-based scoring approach to assess cumulative lifestyle risk factors.

Four lifestyle factors are included in the scoring model:

| Lifestyle Factor | Risk Condition | Weight |
|---|---|---:|
| Sleep Quality | Poor Sleep | 2 |
| Physical Activity | Sedentary | 2 |
| Dietary Habits | Unhealthy Diet | 1 |
| Smoking Status | Smoker | 1 |
| **Maximum Score** | | **6** |

### Risk Score Formula

`Risk Score = (Poor Sleep × 2) + (Sedentary Activity × 2) + (Unhealthy Diet × 1) + (Smoker × 1)`

Each factor contributes points when the corresponding risk condition is present.

### Risk Classification

The resulting scores are classified into three categories:

| Risk Score | Risk Status |
|---:|---|
| 0–1 | Low Risk |
| 2–3 | Moderate Risk |
| 4–6 | High Risk |

### Weighting Rationale

Poor sleep and sedentary physical activity receive higher weights, while unhealthy diet and smoking receive lower weights. This weighting scheme represents an exploratory methodological assumption established for this project to differentiate the contribution of selected lifestyle factors.

The scoring framework is informed by research on cumulative lifestyle factors and composite lifestyle scores. However, the specific weights and classification thresholds used in this project have not been independently validated or clinically established.

Therefore, the resulting categories should be interpreted as exploratory lifestyle risk profiles rather than medical diagnoses or predictions of disease.

## 8. Dashboard Overview

The Power BI dashboard provides an interactive overview of lifestyle-related risk profiles.

### Key Dashboard Features

- **Health Risk Distribution:** Displays the overall distribution of Low, Moderate, and High Risk classifications.
- **Generational Risk Analysis:** Examines risk distributions across different generations.
- **Employment-Based Risk Analysis:** Explores health risk patterns across employment groups.
- **Chronic Condition Analysis:** Compares risk profiles based on chronic condition status.
- **Lifestyle Risk Analysis:** Examines risk distributions across sleep quality, physical activity, dietary habits, and smoking status.
- **Interactive Age Group Filter:** Allows users to explore specific age groups.
- **Key Performance Indicators:** Summarizes population size and the percentage of individuals classified as High Risk.

### Dashboard Preview

<!-- Add your dashboard screenshot below -->

![Lifestyle & Wellness Risk Dashboard](images/dashboard-preview.png)

## 9. Key Findings

The analysis highlights several patterns in the dataset:

1. **Moderate Risk Dominates:** Moderate Risk represents the largest population segment, accounting for approximately 46.5% of the dataset.
2. **Generational Differences:** Seniors account for the highest number of Moderate and High Risk individuals, while Young Adults show a larger proportion of Low Risk classifications.
3. **Sleep Patterns:** Individuals with poor sleep show a substantially higher concentration of High Risk classifications compared with those reporting good sleep.
4. **Physical Activity:** Sedentary individuals have a greater concentration of High Risk classifications, while individuals with moderate or active physical activity show larger Low Risk proportions.
5. **Dietary Habits:** Individuals with unhealthy dietary habits show a higher concentration of Moderate and High Risk classifications than those with healthy dietary habits.
6. **Smoking Status:** Current smokers have a higher proportion of High Risk classifications than non-smokers and former smokers.
7. **Chronic Conditions:** The distribution of risk classifications is relatively similar between individuals with and without reported chronic conditions.

**Interpretation Note:** Risk classifications are constructed from sleep quality, physical activity, dietary habits, and smoking status. Therefore, patterns observed when comparing these same factors against Risk Status are partly determined by the scoring rules themselves. These findings describe the structure of the scoring framework and should not be interpreted as independent evidence of causation.

## 10. Recommendations

Based on the observed patterns, the following initiatives may be considered:

- **Prioritize Moderate Risk Groups:** Develop preventive health awareness initiatives for individuals within the largest risk category.
- **Promote Healthy Sleep and Physical Activity:** Encourage healthier sleep routines and regular physical activity.
- **Improve Dietary Awareness:** Promote balanced dietary habits through education and community-based initiatives.
- **Strengthen Smoking Cessation Programs:** Provide awareness and support programs to encourage smoking cessation.
- **Develop Targeted Preventive Programs:** Consider demographic groups with higher concentrations of risk classifications when planning health promotion activities.

## 11. Potential Impact

This project demonstrates how lifestyle data can be transformed into structured risk profiles to support:

- Population-level lifestyle risk assessment.
- Identification of groups with higher concentrations of risk classifications.
- Data-driven preventive health awareness initiatives.
- More focused health promotion and wellness planning.

## 12. Limitations

Several limitations should be considered when interpreting the results:

- The scoring weights are exploratory assumptions and have not been clinically validated.
- The risk classification thresholds are project-defined rather than established medical standards.
- The analysis identifies patterns and associations, not causal relationships.
- Risk distributions across the scoring components are partly influenced by the scoring formula itself.
- The dataset may not represent all population groups or broader geographic settings.

## 13. References

The following studies provide methodological and conceptual context for cumulative lifestyle scoring and the assessment of lifestyle-related health outcomes:

1. Huang et al. (2025). *Healthy lifestyle habits, educational attainment, and the risk of 45 age-related health and mortality outcomes in the UK: A prospective cohort study.* [DOI: 10.1016/j.jnha.2025.100525](https://doi.org/10.1016/j.jnha.2025.100525)
2. Guasch-Ferré et al. (2022). *Healthy Lifestyle Score Including Sleep Duration and Cardiovascular Disease Risk.* [DOI: 10.1016/j.amepre.2022.01.027](https://doi.org/10.1016/j.amepre.2022.01.027)
3. Gao et al. (2023). *Lifestyle trajectories and ischaemic heart diseases: a prospective cohort study in UK Biobank.* [DOI: 10.1093/eurjpc/zwad001](https://doi.org/10.1093/eurjpc/zwad001)
4. Park et al. (2026). *Healthy Lifestyle Score and the Risk of Cardiovascular Disease, Cancer, and Mortality in an Asian Population: Prospective Cohort Study.* [DOI: 10.2196/95237](https://doi.org/10.2196/95237)

These studies support the relevance of lifestyle factors and composite scoring approaches. They do not establish or validate the exact weights and thresholds used in this project.

## 14. Disclaimer

This project is intended for educational, analytical, and portfolio purposes only. The rule-based risk classifications are exploratory and should not be used as a substitute for professional medical assessment, clinical diagnosis, or individual health recommendations.

## 15. Author

**Zahra Sabilla Usman**

Aspiring Data Analyst | Data Visualization Enthusiast

[LinkedIn Profile](YOUR_LINKEDIN_URL) | [GitHub Profile](YOUR_GITHUB_URL)
