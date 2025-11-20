# Machine-Learning-Project---Christmas-Gift-Price-Prediction


# Correlation between the colums : 
numeric_df = df.select_dtypes(include=['number'])
correlation = numeric_df.corr()
print(correlation)



Price distribution (histogram) : 
The price histogram clearly shows a bias towards the right: most gifts are low to medium priced, with only a few being very expensive. This suggests that a logarithmic transformation of the target price could help stabilise the variance for certain models.

Discount status (countplot) :
The promotional graph shows a significant imbalance: most products do not benefit from discounts, and promotional items generally have lower average prices. The ‘is_discounted’ feature is therefore informative, but insufficient on its own to explain the price.

Price vs volumes (scatter plot) :
The scatter plot representing price versus volume shows no clear trend and virtually no correlation. This indicates that sales volume provides very little guidance for predicting price in this dataset.

Correlation heatmap : 
The correlation heat map reveals strong correlations between certain date-related variables, indicating redundancy (e.g. uk_year1 and uk_year2). Correlations with price are all modest, suggesting that the target depends on a combination of several weakly predictive characteristics rather than a single dominant variable.
