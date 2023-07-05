# Pandas Cheet Sheet

| Method			| Description										| Links and Info	|
|-------------------------------|---------------------------------------------------------------------------------------|-----------------------|
| df.describe() 		| Describe the data									|			|
| df.info() 			| Prints information about the data 							| 			|
| df.head() 			| Prints the starting few rows of data 							| 			|
| df.columns 			| List of column headers as a Series 							| 			|
| df.columns.tolist() 		| List of column headers as a list 							| 			|
| df.shape			| Returns the shape of the data (row x columns)						|			|
| df.iloc[:,:]			| Select rows/columns by index 								| [link](https://sparkbyexamples.com/pandas/pandas-difference-between-loc-vs-iloc-in-dataframe/) |
| df.loc[:,:]			| Select rows/columns by lables								| [link](https://sparkbyexamples.com/pandas/pandas-difference-between-loc-vs-iloc-in-dataframe/) |
| df.isnull()			| Detect missing values in the data    							|			|
| df.isna()			| Same as isnull, detect missing values							|			|
| df.dropna(axis=0/1)		| Drop rows/columns containing missing values						|			|
| df.columns[data.isna().any()] | List of columns with missing data 							|			|
| df.fillna(value=values)	| Fill na values with a specified dict values						|			|
| df.mode()			| Gives the mode (most frequently occuring value) in each column			|			|
| df[col].fillna(df[col].mode()[0], inplace=True | Fill the na values in a column with its mode value			|			|
| df.replace({col: dict})	| Replace values in the specified col with specified dict values			| [link](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.replace.html)|
| df.drop_duplicates()		| Remove any duplicate rows	      	   	     	  				|			|
| df.corr()			| Returns pairwise correlation matrix 							|			|
| df.corrwith(col)		| Returns correlation with a particular column						|			|
