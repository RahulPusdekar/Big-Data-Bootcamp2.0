# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?

import pandas as pd
df = pd.read_csv("file_path")

Q2. How do you check the data type of a column in a Pandas DataFrame?

using dtypes attribute

Q3. How do you select rows from a Pandas DataFrame based on a condition?

selected_rows1 = dataframe[dataframe['column_name'] > 78]
selected_rows2 = dataframe[(dataframe['column_name'] > 78) & (dataframe['column_name'] == 'rahul')]


Q4. How do you rename columns in a Pandas DataFrame?
# Rename using rename()
df.rename(columns = {'old_ColumnName':'new_ColumnName', inplace=True})

# Rename all columns by assigning new list of column
df.columns = ['list of all new_column_names']


Q5. How do you drop columns in a Pandas DataFrame?

df.drop('column_name', axis=1)

Q6. How do you find the unique values in a column of a Pandas DataFrame?

# using unique() method
df.column_name.unique()

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
Ans: df.isna().sum()

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
Ans: using fillna() method

Q9. How do you concatenate two Pandas DataFrames?
Ans: using concat() with appropriate 'axis' parameter

Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: using merge()

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
Ans: using groupby()

Q12. How do you pivot a Pandas DataFrame?
Ans: using pivot_table()

Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans: using astype()

Q14. How do you sort a Pandas DataFrame by a specific column?
Ans: using sort_values() 

Q15. How do you create a copy of a Pandas DataFrame?
Ans: using copy()

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans: We can use the loc[] method and the & or | operator to combine multiple conditions.

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
Ans: using mean()

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
Ans: using std()

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
Ans: using corr()

Q20. How do you select specific columns in a DataFrame using their labels?
Ans: using []. For, example df['column_label']

Q21. How do you select specific rows in a DataFrame using their indexes?
Ans: using iloc[]

Q22. How do you sort a DataFrame by a specific column?
Ans: using sort_values()

Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans: Example, df['new_column'] = df['column1'] - df['column2'] 

Q24. How do you remove duplicates from a DataFrame?
Ans: using drop_duplicates()

Q25. What is the difference between .loc and .iloc in Pandas?
Ans: .loc is used to select rows and columns based on their label values whears .iloc is used to select rows and columns based on their integer position(index)