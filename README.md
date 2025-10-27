# Landing Page A/B Test Analysis
This project analyzes data from a landing page A/B test to evaluate whether a new page improved user conversions compared to the old one.  
The dataset is from Kaggle’s Udacity A/B testing exercise.

## Project Summary
The goal is to check if the new landing page led to higher conversion rates.  
After cleaning mismatched and duplicate entries, conversion rates were calculated and compared using a two-proportion z-test.  
95% confidence intervals were also computed to assess statistical significance.  
A sample size check (MDE) confirmed that the dataset was large enough to detect small differences.

## Results
- Control group conversion rate: 12.04%
- Treatment group conversion rate: 11.88%  
- p-value: 0.19 (no statistically significant difference)  
- 95% Confidence Intervals overlap -- performance difference likely due to random variation.  
- The sample size (~145K per group) -- sufficient for detecting small effects.

Conclusion:  
No evidence that the new landing page performs better; the current version should remain live unless a new, substantially different variant is introduced.

## Tools Used
- Python: Pandas, NumPy, Matplotlib, SciPy  
- Environment: Jupyter Notebook  
- Dataset: [Kaggle - Udacity A/B Test Dataset](https://www.kaggle.com/datasets)

## Workflow
- Data cleaning and validation  
- Exploratory data analysis  
- Hypothesis testing (two-proportion z-test)  
- Confidence interval estimation  
- Sample size and MDE evaluation  
- Interpretation and recommendation