# Parkinsons longitudinal disease severity modeling with mixed-effects analysis
## Overview
I modeled how disease severity evolves over time using mixed-effects models, which account for repeated visits per patient. I found that disease severity increases significantly over time, but with large variability across patients, meaning progression rates differ widely

The goal was to understand how disease severity changes over time using repeated clinical visits, rather than treating each observation independently.

This kind of modeling is important for predicting disease progression, evaluating treatment effectiveness, and identifying high-risk patients

I built a full pipeline including data cleaning, longitudinal formatting, feature engineering, mixed-effects modeling, and visualization

## Data used
I used the MDS-UPDRS Part III longitudinal data from the PPMI dataset, which includes multiple clinical visits per patient. I focused on the MDS-UPDRS Part III score as a measure of disease severity.

## How is this different from typical ML problems?
The challenge is that observations from the same patient are not independent, so standard regression would give biased results.

## Method
I used a linear mixed-effects model, which separates population-level effects from patient-specific variability. This allowed me to model both the average progression and individual patient trajectories

