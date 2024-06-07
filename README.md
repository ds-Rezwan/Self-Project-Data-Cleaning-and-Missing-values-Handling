# Self-Project-Data-Cleaning-and-Missing-values-Handling
Data cleaning and missing values handling are crucial to preparing data for analysis. These tasks can be efficiently managed using Pandas in Python with various built-in functions. This project has been completed using pandas in Python. here's a summary:
# Data Loading:
df=pd.read_csv('dirty data.csv')
# df.isna() and df.isna().sum()
df.isna(): method checks whether the objects of a Dataframe or a Series contain missing or null values (NA, NaN) and returns a new object with the same shape as the original but with boolean values True or False as the elements. True indicates the presence of null or missing values and False indicates otherwise.

The sum(): function returns the sum of True values, which equals the number of NaN values in the column.
# Dropna()
The drop() method removes the specified row or column. By specifying the column axis ( axis='columns' ), the drop() method removes the specified column. By specifying the row axis ( axis='index' ), the drop() method removes the specified row.
# Fillna():
The fillna() method replaces the NULL values with a specified value. The fillna() method returns a new DataFrame object unless the inplace parameter is set to True , in that case the fillna() method does the replacing in the original DataFrame instead.
# Boxplot:
Make a box-and-whisker plot from DataFrame columns, optionally grouped by some other columns. A box plot is a method for graphically depicting groups of numerical data through their quartiles.
# duplicated values
You can count duplicate rows by counting True in the Series returned by duplicated() . True can be counted with the sum() method. print(df. duplicated(). sum()).
# Replace()
We use the replace() function to replace the string “Python” with the string “Java”. The replace() function returns a new string with the replacements made, which we store in the variable new_s . Finally, we print the value of new_s , which will be: “I love Java programming.
# inplace(): 
In general, functions are used when we want to perform an operation on an object and get a result, while in-place operations are used when we want to modify an object directly without getting a result.
# iloc()
It allows the selection and retrieval of specific rows and columns in DataFrames or Series using integer-based indexing. iloc() allows to identification data by specifying row and column indices numerically. For instance, df. iloc[0] retrieves the first row, while df.

