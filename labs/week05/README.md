**Program 1: Sensor Data Matrix Analysis**
**Overview**

This program analyzes simulated sensor readings collected from 4 machines over 5 time intervals using NumPy arrays. Each row represents a machine, and each column represents a time interval.

The program performs statistical analysis, normalization, reshaping, and conditional filtering using NumPy operations.

**Implemented Operations**

Computed average reading per machine using row-wise axis operations

Computed maximum reading per time interval using column-wise axis operations

Normalized the matrix using broadcasting by dividing each value by its column maximum

Identified machines where the average reading is greater than 20 using boolean indexing

Reshaped the original matrix into a new shape of (2, 10)

**Key Concepts Practiced**

Axis-based aggregation (axis=0, axis=1)

NumPy broadcasting

Matrix reshaping

Boolean indexing and filtering

Vectorized numerical computation

**Program 2: Matrix Combination & Filtering**
**Overview**

This program demonstrates matrix operations using randomly generated 3×3 matrices. It focuses on both linear algebra operations and element-wise operations, along with filtering and stacking techniques.

Implemented Operations

Generated two 3×3 matrices with random integers

Performed matrix multiplication using the @ operator

Performed element-wise multiplication

Extracted values greater than 100 from the matrix multiplication result using boolean masking

Replaced elements less than 10 in the original matrices with 0

Vertically stacked both matrices into a larger matrix

**Key Concepts Practiced**

Matrix multiplication vs element-wise multiplication

Boolean masking

Conditional replacement

Matrix stacking (vstack)

Efficient numerical computation using NumPy

**Challenges Faced**

Understanding the difference between axis 0 and axis 1 operations

Applying broadcasting correctly for normalization

Distinguishing between matrix multiplication and element-wise multiplication

Managing reshaping without altering total element count

Data Analysis Lab (NumPy & Pandas)
1. Difference Between NumPy and Pandas Usage in This Lab

In this lab, both NumPy and Pandas were used for different purposes in data analysis.

NumPy was mainly used for numerical and matrix operations. It allows fast mathematical computations on arrays. In this lab, NumPy was used to perform operations such as matrix multiplication, element-wise multiplication, broadcasting, reshaping arrays, and stacking matrices.

Pandas, on the other hand, was used for data manipulation and analysis of tabular data. It provides the DataFrame structure, which is similar to a table or spreadsheet. In this lab, Pandas was used to clean data, handle missing values, filter rows, group data, compute statistics, create pivot tables, and export datasets to CSV files.

In simple terms:

NumPy → Numerical and matrix computations

Pandas → Data analysis and data manipulation

2. Why Vectorization is Preferred Over Loops

Vectorization means performing operations on entire arrays or columns at once instead of processing each element using loops.

Vectorized operations are preferred because:

Faster execution: NumPy and Pandas are optimized in C internally, making operations much faster than Python loops.

Less code: Vectorized operations require fewer lines of code, making the program simpler and easier to read.

Better performance on large datasets: When working with large datasets, loops become slow, while vectorized operations handle data efficiently.

For example:

Loop approach (slower):

for i in range(len(data)):
    data[i] = data[i] * 1.15

Vectorized approach (faster):

df["TaxedAmount"] = df["Amount"] * 1.15

The vectorized approach processes the entire column at once, which improves performance.

3. How Missing Data Was Handled

In the dataset, the Amount column contained missing values (None). Missing data can cause errors during calculations and analysis, so it must be handled properly.

In this lab, missing values were handled using the median value of the Amount column.

Steps used:

Detect missing values using isnull().

Calculate the median of the Amount column.

Replace missing values using fillna().

Example:

df["Amount"] = df["Amount"].fillna(df["Amount"].median())

Using the median is useful because it is less affected by extreme values compared to the mean. This ensures that the dataset remains balanced and suitable for further analysis