# Machine-Learning-Project---Christmas-Gift-Price-Prediction


# Correlation between the colums : 
numeric_df = df.select_dtypes(include=['number'])
correlation = numeric_df.corr()
print(correlation)

## Correlation Analysis

The correlation matrix shows linear relationships between numerical variables in the dataset.

### Key Points:

- **Most variables**: weak correlations → features are largely independent.
- **Strong relationships among some LSG variables**:
  - `lsg_1 ↔ lsg_3 = 0.53`
  - `lsg_4 ↔ lsg_6 = 0.36`
  These variables capture similar information.
- **Gift type influence**:
  - `gift_type` is moderately correlated with `lsg_1` and `lsg_3`.
- **Price and discount**:
  - `is_discounted ↔ price = -0.22` → discounted products tend to have lower prices.
- **Volumes and price**:
  - Very weak correlation `0.037` → price does not strongly affect quantity sold.
- **Year-related variables**:
  - `uk_year1 ↔ uk_year2 = 0.93` → very strong similarity.
  - Other year columns → weak correlations with the rest.

**Conclusion:** Few strong linear relationships exist, but watch out for redundancy among some LSG and year columns.

