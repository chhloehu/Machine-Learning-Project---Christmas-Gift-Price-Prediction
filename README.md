# Machine-Learning-Project---Christmas-Gift-Price-Prediction


# Correlation between the colums : 
numeric_df = df.select_dtypes(include=['number'])
correlation = numeric_df.corr()
print(correlation)
