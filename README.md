# AB_testing_ecommerce
Statistical A/B test on an e-commerce dataset (Python, pandas, statsmodels)
Author: Chaou Khadidja Nihel  
Master 1 in Statistics — A/B Testing Project  

This project analyzes an "A/B test" conducted on an "e-commerce website" to determine whether a new webpage design increases the conversion rate compared to the old version.

The analysis uses Python and statistical testing methods to make "data-driven decisions"

Dataset
- Source: [E-commerce A/B Testing Dataset (Kaggle)](https://www.kaggle.com/datasets/ahmedmohameddawoud/ecommerce-ab-testing)  
- Rows: 294,478 users  
- Columns:
  - 'id' = user identifier  
  - 'time' = visit time  
  - 'con_treat' = group assignment ('control' or 'treatment')  
  - 'page' = page type ('old_page' or 'new_page')  
  - 'converted' = 1 if the user converted, 0 otherwise 

Methodology
The analysis follows these steps:
1. "Data Cleaning:" remove duplicates, inconsistent records.  
2. "Exploratory Analysis:" visualize conversion rates and group balance.  
3. "Statistical Testing:"
   - Two-Proportion "Z-Test"
   - "Chi-Square Test"
   - "Logistic Regression"
   - "Bootstrap Confidence Intervals"
4. "Power Analysis:" determine the required sample size to detect small effects.

Statistical Results
| Test | Result | Interpretation |
|------|---------|----------------|
| Two-Proportion Z-Test | p = 0.216 | Not significant |
| Chi-Square Test | p = 0.192 | Not significant |
| Logistic Regression | OR = 0.985 | Treatment slightly lower but not significant |

- "Control Conversion Rate:" 12.04%  
- "Treatment Conversion Rate:" 11.89%  
- "Difference:" −0.15%  
- "95% CI:" [−0.38%, +0.09%]  

Conclusion
- The statistical tests show "no significant difference" between the old and new pages.  
- The new design does "not significantly improve" user conversions.  
- Therefore, we recommend "keeping the current (control) version" of the webpage.

