# Summary of Univariate and Multivariate Logsitic Regression Analysis for Leukmia Risk Factors

This project investigated potential risk factors associated with Leukemia Status using logistic regression analysis. Both univariate and multivariate approaches were employed to assess the relationship between several numerical and categorical risk factors and the binary outcome of Leukemia Status.

## univariate Logsitic Regression Analysis

Univariate logsitic regression was performed for each of the following numerical risk factors:

- `WBC_Count`.
- `Bone_Marrow_Blasts`.
- `Age`.
- `RBC_Count`.
- `BMI`.

The results from the univariate analysis, summarized in the forest plot, indecate that **none of these numerical risk factor demonstrated a statistically significant association with Leukemia Status at a significance level of a = 0.05**.

For each numerical risk factor, the Odds Ratio (OR) was close to 1.0, and the 95% Confidence Invervals (CIs) consistently spanned 1, visually confirming the lack of statistically significant univariate effects. While `Bone_Marrow_Blast` exhibited a slightly elevated OR and a p-value nearing significance (p ≈ 0.088), it did not reach the conventional statistical significance threshold.

Furthomore, univariate regression analysis for categorical risk factors: 

- `Smoking_Status_Yes` 
- `Family_History_Yes` 
- `Genetic_Mutation_Yes` 
- `Ethnicity_Ethnic_Group_B` 
- `Ethnicity_Ethnic_Group_C` 
- `Socioeconomic_Status_Low` 
- `Socioeconomic_Status_Medium` 

was limited due to zero variance in these categorical variables within the dataset. Consequently, these categorical factors were excluded from the univariate regression model.

## Multivariate Logsitic Regression Analysis

To assess the independent effects and potential confounding among numerical risk factors, a multivariate logistic regression model was constructed, including `Bone_Marrow_Blasts`, `Age`, `WBC_Count`, `RBC_Count`, and `BMI` simultaneously.

The comparison bar plot visually represents the comparison between univariate and multivariate Odds Ratios for these numerical factors. Notably, the adjusted Odds Ratios (**aORs**) from the multivariate model remained very similiar to the univariate ORs, and again, **no factor reached statiscal significance in the multivariate context (p < 0.05)**.

## key Findings and Interpretations

- **Lack of Statistically Risk Factors:** Both univariate and multivariate logsitic regression analysis, conducted on this dataset, failed to identify statistically significanct associations between the investigated numerical risk factors and Leukemia Status.

- **Consistent Result Across Analyses:** the consistency between univariate and multivariate findings, visually supported by the comparison bar plot, suggest that confounding among the examined numerical risk factors is minimal in this dataset and model spesification.

- **Bone_Marrow_Blasts: Potential Trend:** While not statistically significant `Bone_Marrow_Blasts` exhibited a slightly elevated Odss Ratio in both analyses, warranting consideration for further investigation in larger dataset or with different analytical approaches.

- **Categorical Variables with Zero Variance:** Categorical risk factors could not be analyzed in this dataset due to a lack of variability, highlighting a limitation of the data for asessing these factors.

## Conclusion

In conclusion, based on the logistic regression analyses of this dataset, there is **no strong statistical evidence to support a significant association between the examined numerical risk factors (WBC_Count, Bone_Marrow_Blasts, Age, RBC_Count, BMI) and Leukemia_Status.** While Bone_Marrow_Blasts showed a trend towards incresed Odds of Leukemia Status, this finding did not reach statistical significance and require further investigation. The categorical risk factors could not evaluated due to data limitations.

Further research may be warranted, potentially with larger and more diverse datasets, to explore these and other potential risk factors for Leukemia Status more comprehensively. Alternative modeling approaches or investigation of variable interactions might also yield further insights.