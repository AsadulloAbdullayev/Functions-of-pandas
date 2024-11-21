# Pandas Functions
This repository is dedicated to the most commonly used functions of the pandas library. Pandas is one of the most popular libraries in Python for data analysis and manipulation. This repository showcases the main functions of the pandas library, how they work, and provides examples. It is a valuable resource for developers and researchers working in the field of data analysis.

## List of Contents
### 1. Functions for Data Creation and Importing
- `pd.DataFrame()`: Creating a DataFrame object.
- `pd.Series()`: Creating a Series object.
- `pd.read_csv()`: Reading data from a CSV file.
- `pd.read_excel()`: Reading data from an Excel file.
- `pd.read_sql()`: Retrieving data from a database using SQL queries.
- `pd.read_json()`: Reading data from a JSON file.

### 2. Information about DataFrame
- `df.info()`: Retrieving general information about the DataFrame.
- `df.describe()`: Statistical information for numerical columns.
- `df.shape`: Returns the number of rows and columns in the DataFrame.
- `df.columns`: Retrieve column names in the DataFrame.
- `df.index`: Retrieve DataFrame indices.

### 3. Data Selection and Filtering
- `df.head(n)`: Shows the first n rows.
- `df.tail(n)`: Shows the last n rows.
- `df[["col1", "col2"]]`: Select specific columns.
- `df.iloc[]`: Select rows and columns by index.
- `df.loc[]`: Select rows and columns by index or column name.
- `df[df["column"] > value]`: Filter data by column value.
- `df.at[]`: Fast access to scalar values.
- `df.iat[]`: Fast access using integer indices.

### 4. Data Cleaning
- `df.dropna()`: Drop rows with missing values (NaN).
- `df.fillna(value)`: Fill missing values with a specified value.
- `df.drop_duplicates()`: Drop duplicate rows.
- `df.replace()`: Replace specific values with other values.
- `df.astype()`: Change the data type of a column.

### 5. Data Transformation
- `df.apply()`: Apply a function along an axis of the DataFrame.
- `df.map()`: Apply a function to each element in a Series.
- `df.applymap()`: Apply a function to each element.
- `pd.factorize()`: Encode categorical values.
- `df.rename()`: Rename columns or indices.
- `df.sort_values()`: Sort data by values.
- `df.sort_index()`: Sort data by index.

### 6. Grouping and Aggregation Functions
- `df.groupby()`: Group data.
- `df.agg()`: Compute aggregates like sum, mean, etc.
- `df.crosstab()`: Create a cross-tabulation table between two columns.
- `df.value_counts()`: Count the frequency of values in a column.
- `df.transform()`: Transform data.
- `df.pipe()`: Apply functions sequentially.

### 7. Statistical Functions
- `df.mean()`: Calculate the mean value.
- `df.median()`: Calculate the median value.
- `df.mode()`: Calculate the mode value.
- `df.min(), df.max()`: Get the minimum and maximum values.
- `df.std(), df.var()`: Standard deviation and variance.
- `df.corr()`: Calculate correlation coefficient.
- `df.cov()`: Calculate covariance.

### 8. Merging Data
- `pd.concat()`: Concatenate DataFrame or Series objects.
- `pd.merge()`: Merge two DataFrame objects.
- `df.join()`: Join on indices.

### 9. Time and Date Management
- `pd.to_datetime()`: Convert data to datetime type.
- `df.resample()`: Resample time-series data.

### 10. Working with Datetime
- `df['date'].dt.year, df['date'].dt.month, df['date'].dt.day`: Extract year, month, or day from date.
- `df['date'].dt.weekday`: Get the day of the week.
- `df['date'].dt.is_month_end`: Check if it's the end of the month.
- `df['date'].dt.is_leap_year`: Check if it's a leap year.

### 11. Data Export and Saving
- `df.to_csv()`: Save DataFrame to a CSV file.
- `df.to_excel()`: Save DataFrame to an Excel file.
- `df.to_sql()`: Save data to an SQL database.
- `df.to_json()`: Save DataFrame to a JSON file.

### 12. Indexing Operations
- `df.set_index()`: Set a specified column as the index.
- `df.reset_index()`: Reset the index.
- `df.reindex()`: Reindex the DataFrame.
- `df.index.name`: Change or retrieve index name.

### 13. Mathematical and Logical Operations
- `df.add(), df.sub(), df.mul(), df.div()`: Perform addition, subtraction, multiplication, and division.
- `df.abs()`: Get absolute values.
- `df.round()`: Round numbers.
- `df.clip(lower, upper)`: Clip values at specified limits.
- `df.cumsum()`: Cumulative sum.
- `df.cumprod()`: Cumulative product.

### 14. String Functions (For object or str columns only)
- `df['column'].str.contains()`: Check if a specific value exists.
- `df['column'].str.startswith(), df['column'].str.endswith()`: Check if text starts or ends with a specific value.
- `df['column'].str.lower(), df['column'].str.upper()`: Convert text to lower or upper case.
- `df['column'].str.replace()`: Replace specified values.
- `df['column'].str.split()`: Split text by a specified delimiter.
- `df['column'].str.strip()`: Remove leading and trailing spaces.

### 15. Moving Window and Rolling Functions
- `df.rolling(window)`: Create rolling statistics.
- `df.expanding()`: Create expanding statistics.

### 16. Time Series Functions
- `df.asof()`: Get the value closest to a specified date.
- `df.shift()`: Shift rows or columns.
- `df.diff()`: Calculate the difference.


### 17. Style and Formatting
- `df.style`: Provides a way to style a DataFrame.
- `df.style.highlight_max()`: Highlight maximum values.
- `df.style.highlight_min()`: Highlight minimum values.
- `df.style.set_precision()`: Set the number precision.

### 18. Miscellaneous Useful Functions
- `df.memory_usage()`: Get memory usage of a DataFrame.
- `df.query()`: Perform SQL-like queries on DataFrame.
- `pd.qcut()`: Quantile-based discretization.
- `pd.cut()`: Discretize values into bins.
- `pd.factorize()`: Encode categorical values.
- `df.melt()`: Convert wide format to long format.
- `df.explode()`: Transform each element of a list-like to a row.

### 19. Working with Categories
- `df['column'].astype('category')`: Convert column to category.
- `df['column'].cat.add_categories()`: Add new categories.
- `df['column'].cat.remove_categories()`: Remove specified categories.
- `df['column'].cat.rename_categories()`: Rename categories.
- `df['column'].cat.codes`: Get the category codes.

### 20. Sparse Data (Optimized Storage)
- `pd.SparseArray()`: Create a sparse array.
- `pd.SparseDtype()`: Set dtype for sparse data.
- `df.sparse.density`: Check the density of sparse data.

### 21. MultiIndex Operations. Pivot and Reshape Functions
- `df.unstack()`: Unstack a level of index.
- `df.stack()`: Stack a level of columns.
- `df.swaplevel()`: Swap levels of a MultiIndex.
- `df.droplevel()`: Drop a level from a MultiIndex.
- `df.reorder_levels()`: Reorder levels of a MultiIndex.
- `df.pivot()`: Reshape DataFrame.
- `df.pivot_table()`: Create pivot table with aggregation.
- - `df.xs()`: Select a cross-section from a DataFrame.

### 22. Window Functions
- `df.rolling(window=3).sum()`: Calculate rolling sum with a 3-row window.
- `df.expanding().mean()`: Calculate expanding mean.
- `df.ewm(alpha=0.5).mean()`: Calculate exponentially weighted mean.

### 23. Targeted Statistical Functions
- `df.kurtosis()`: Calculate kurtosis.
- `df.skew()`: Calculate skewness.
- `df.mad()`: Mean absolute deviation.
- `df.sem()`: Standard error of the mean.

### 24. Working with NaN and NULL
- `df.notna()`: Check for non-NaN values.
- `df.isnull()`: Check for NaN values.
- `df.interpolate()`: Fill NaN values by interpolation.

### 25. Checking DataFrame Structure and Object Types
- `df.empty`: Check if DataFrame is empty.
- `df.size`: Get the number of elements.
- `df.ndim`: Get the number of dimensions.
- `df.dtypes`: Show data types of columns.
- `df.memory_usage(deep=True)`: Show memory usage in detail.

### 26. Other Utility Functions
- `df.eval()`: Perform expressions on DataFrame.
- `df.query()`: Perform SQL-like queries on DataFrame.
- `pd.get_dummies()`: One-hot encoding.
- `df.style.applymap()`: Apply styling to each cell.
- `pd.interval_range()`: Create an interval range.
- `df.equals()`: Check if two DataFrames are equal.

### 27. Diagnosis and Diagnostic Functions
- `pd.show_versions()`: Show versions of pandas and its dependencies.
- `pd.get_option(), pd.set_option()`: Get and set pandas options.
- `pd.reset_option()`: Reset pandas options to defaults.
- `pd.describe_option()`: Show all available parameter options.
- `df.memory_usage()`: Get memory usage of a DataFrame.

### 28. Advanced Category Handling
- `df['column'].cat.set_categories()`: Set specific categories.
- `df['column'].cat.as_ordered()`: Set category as ordered.
- `df['column'].cat.reorder_categories()`: Reorder categories.
- `df['column'].cat.remove_unused_categories()`: Remove unused categories.

### 29. Profiling and Data Statistics
- `pd.util.testing.assert_frame_equal()`: Test if two DataFrames are equal.
- `pd.util.testing.assert_series_equal()`: Test if two Series are equal.
- `df.profile_report()`: Create a comprehensive profile report.

### 30. Data Quality Checking and Cleaning
- `df.isin()`: Check DataFrame against given values.
- `df.eval()`: Efficiently evaluate expressions on DataFrame.
- `df.mask()`: Hide or transform values based on condition.
- `pd.to_numeric()`: Convert to numeric type.

### 31. Working with Large DataFrames
- `df.memory_usage(deep=True)`: Show memory usage.
- `pd.read_csv(chunksize=n)`: Read large CSV files in chunks.
- `df.to_parquet(), pd.read_parquet()`: Save and read data in Parquet format.

### 32. Advanced Sparse Data Handling
- `pd.arrays.SparseArray()`: Create sparse arrays.
- `pd.SparseDataFrame()`: Create DataFrame for sparse data.
- `df.sparse.from_dense()`: Convert dense to sparse DataFrame.
- `df.sparse.to_dense()`: Convert sparse to dense.

### 33. Working with Interval Values
- `pd.Interval()`: Define a single interval.
- `pd.IntervalIndex()`: Create an index of intervals.

### 34. Advanced Numeric Functions
- `pd.Series.rank()`: Rank values in Series.
- `df.corrwith()`: Compute correlation with another Series or DataFrame.
- `df.rank()`:: Rank the DataFrame values.

### 35. Advanced Merging and Join Operations
- `pd.merge_ordered()`: Ordered merge of two DataFrames.
- `pd.merge_asof()`: Merge based on closest match.
- `df.update()`: Update DataFrame values with new ones.


### 36. Vectorization Functions
- `df.apply(np.vectorize(function))`: Apply a function element-wise.
- `df.applymap(np.vectorize(function))`: Apply a function to each DataFrame element.

### 37. Diagnostics and DataFrame Creation Functions
- `pd.util.hash_pandas_object()`: Hash a DataFrame or Series.
- `pd.array()`: Create a pandas array.
- `pd.interval_range()`: Create an interval index range.

These functions help to unlock the full potential of the Pandas library for efficient data manipulation, transformation, analysis, and cleaning. If you need a more detailed explanation or examples for any specific function, please let me know!
