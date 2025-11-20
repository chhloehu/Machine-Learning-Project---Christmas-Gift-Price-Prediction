# Machine-Learning-Project---Christmas-Gift-Price-Prediction


# Correlation between the colums : 
numeric_df = df.select_dtypes(include=['number'])
correlation = numeric_df.corr()
print(correlation)

Interpretation of the correlation results : 

The correlation matrix shows that most variables have weak relationships, meaning they are largely independent. The strongest links are between some LSG variables (especially lsg_1 with lsg_3 and lsg_4 with lsg_6), indicating they capture similar information. gift_type also shows moderate correlations with some LSG features. As expected, discounted items tend to have lower prices, while price and volumes show almost no relationship. Overall, only a few feature pairs are strongly related.
