# Machine-Learning-Project---Christmas-Gift-Price-Prediction


# Correlation between the colums : 
numeric_df = df.select_dtypes(include=['number'])
correlation = numeric_df.corr()
print(correlation)

Interpretation of the correlation results : 

Most variables show weak correlations, so features are largely independent.
Strong correlations exist among some LSG variables:
  lsg_1 ↔ lsg_3 = 0.53
  lsg_4 ↔ lsg_6 = 0.36
These variables may capture similar information.
gift_type moderately correlates with lsg_1 and lsg_3, indicating gift type influences these metrics.
Discounted items are slightly associated with lower prices (is_discounted ↔ price = -0.22).
Volumes and price are almost uncorrelated (0.037), so price doesn’t strongly affect quantity sold.
Year variables are mostly independent, except uk_year1 ↔ uk_year2 = 0.93, showing strong similarity.
Overall: Few strong linear relationships exist; most features are independent, with some redundancy among LSG variables and year columns.
