# pandas
Q1. How do you load a CSV file into a Pandas DataFrame?
Ans: 
import pandas as pd
df = pd.read_csv('file_name.csv')
print(df)

Q2. How do you check the data type of a column in a Pandas DataFrame?
Ans:

In pandas dataframe , we can use the “dtype” attribute it returns a series with data type of each column.
Ex:
Result = df.dtypes

Q3. How do you select rows from a Pandas DataFrame based on a condition?
Ans: 
df= pd.DataFrame(record , column[name1,name2])
result_df = dataframe[dataframe[‘name’>80]]

Q4. How do you rename columns in a Pandas DataFrame?
Ans: We can rename a column in pandas dataframe using rename() function.

df.rename(columns = {'Name':'name'},inplace=True)
print(df.columns)

Q5. How do you drop columns in a Pandas DataFrame?
Ans: we can drop a column in pandas DataFrame using drop() method of Pandas.

Q6. How do you find the unique values in a column of a Pandas DataFrame?
Ans: We can find the unique values in a column of a a Pandas DataFame using the unique() method.

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
Ans: We can find number of missing values in each column of a pandas dataframe using isnull()

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
Ans: We can fill missing value in a Pandas DataFrame with a specific value using the fillna() method.

Q9. How do you concatenate two Pandas DataFrames?
Ans: We will pass two dataframes to pd.concat() method in the form of a list and mention the axis. Axis=0 to concat along rows and Axis=1 to concat along columns.

Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: We can merge two Panda DataFrame on a specific column with the merge method.
Ex: 
Imagine two dataframes DF1 and DF2 

DF1.merge(DF2[[‘col1’,’col2’]])

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
Ans: We can group data in panda DataFrame by a specific column using groupby() method and get aggregation using the agg() method.
Ex:
Group_by = df.groupby(“column_name”).agg({‘column’:[‘min’,’max’,’’mean]}) 

Q12. How do you pivot a Pandas DataFrame?
Ans: Pivot() function is used to reshape a given dataframe organized by index/column values.

Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans: The astype() method function is used to dataframe into a particular data type. And for a column we have to pass a key value pair dictionary with column name and data type to cast the column into a particular data type.
Ex:
Convert_datatype = {‘column_name’: data type}
Df = df.astype(Convert_datatype)

Q14. How do you sort a Pandas DataFrame by a specific column?
Ans : We can sort a pandas dataframe using a sort_values() method.
Ex:
Df.sort_values(by=[‘column_name’])

Q15. How do you create a copy of a Pandas DataFrame?
Ans: Copy() method returns a copy of the dataframe.


Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans: We can filter rows of pandas dataframe using the loc and query method.

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
Ans : We use the mean() method to calculate the mean of a column in pandas dataframe.

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
Ans: we can calculate standard deviation using std() method.


Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
Ans: By using corr() we can find the correlation between two columns in a Panda DataFrame.

Q20. How do you select specific columns in a DataFrame using their labels?
Ans: Using the loc method we can select specific columns in dataframe.


Q21. How do you select specific rows in a DataFrame using their indexes?
Ans: we can select using specific rows in a dataframe using their indexes by using the iloc method.

Q22. How do you sort a DataFrame by a specific column?
Ans: using the sort_values() method


Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans: we can create a new column in a DataFrame based on values of the another column by using the apply() method.


Q24. How do you remove duplicates from a DataFrame?
Ans: using the drop_duplicates() method.


Q25. What is the difference between .loc and .iloc in Pandas?
Ans: loc get the dataframes rows and columns by labels and names , while iloc uses the indexing of the rows and columns.


