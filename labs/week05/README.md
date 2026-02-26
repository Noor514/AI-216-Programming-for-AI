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