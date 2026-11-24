# Tholkapian_N_PATP_exp01    
# Experiment-1-Exploring-NumPy-and-Pandas

## Aim

To understand the use of NumPy and Pandas for performing basic data
manipulation and analysis in Python.

## Algorithm
1. Import the NumPy library for numerical and array operations and the Pandas library for data manipulation and analysis.
2. Create two NumPy arrays, arr1 and arr2, containing numerical values.
3. Perform arithmetic operations on the arrays:
   - Addition using arr1 + arr2.
   - Subtraction using arr1 - arr2.
   - Multiplication using arr1 * arr2.
   - Division using arr1 / arr2.
4. Define a dictionary data containing employee details such as Name, Age, and Salary.
5. Convert the dictionary into a Pandas DataFrame using pd.DataFrame(data).
6. Display the DataFrame to view the employee dataset.
7. Calculate descriptive statistical measures such as count, mean, standard deviation, minimum, maximum, and quartiles using df.describe().
8. Display the DataFrame information using df.info() to identify column names, data types, non-null values, and memory usage.
9. Display all the results.
10. End the program.
## Formulas / Theory
- NumPy Array Creation:
\[
A = [a_1,a_2,a_3,\ldots,a_n]
\]

- Addition:
\[
C_i = A_i+B_i
\]

- Subtraction:
\[
C_i = A_i-B_i
\]

- Multiplication:
\[
C_i = A_i\times B_i
\]

- Division:
\[
C_i = \frac{A_i}{B_i}, \quad B_i\neq 0
\]

- Mean (Average):
\[
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
\]

- Standard Deviation:
\[
\sigma=\sqrt{\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}}
\]

- Minimum: Smallest value in the dataset.

- Maximum: Largest value in the dataset.

- Quartiles:
- Q1 = 25th percentile
- Q2 = 50th percentile (Median)
- Q3 = 75th percentile
- DataFrame: A two-dimensional tabular data structure consisting of rows and columns.

- Descriptive Statistics: Used to summarize and understand the characteristics of numerical data.
## Coding
# Input 1
```
import numpy as np
import pandas as pd
  # step 1: Numpy Array Operation
arr1=np.array([10,20,30,40,50])
arr2=np.array([2,4,6,8,10])
print("A:",arr1)
print("B:",arr2)
#Arthimetic Operation
print("Addition:",arr1+arr2)
print("Subtraction:",arr1-arr2)
print("Multiplication:",arr1*arr2)
print("Division:",arr1/arr2)
```
## Output 1
```
A: [10 20 30 40 50]
B: [ 2  4  6  8 10]
Addition: [12 24 36 48 60]
Subtraction: [ 8 16 24 32 40]
Multiplication: [ 20  80 180 320 500]
Division: [5. 5. 5. 5. 5.]
```
## Input 2
```
#Step 2: Pandas dataframe
data={
    'Name':["Nagaraj","Santhosh","Divya Bharathi","Thirshal Shalini"],
    'Age':[22,23,24,25],
    'Salary': [40000,42000,38000,34000]
}
df=pd.DataFrame(data)
# display Data
print("\nDataset:")
print(df)
# Descriptive statistics
print("\nStatistical Summary:")
print(df.describe())
print("\nData Info:")
print(df.info())
```
## Output 2
```
Dataset:
               Name  Age  Salary
0           Nagaraj   22   40000
1          Santhosh   23   42000
2    Divya Bharathi   24   38000
3  Thirshal Shalini   25   34000

Statistical Summary:
             Age        Salary
count   4.000000      4.000000
mean   23.500000  38500.000000
std     1.290994   3415.650255
min    22.000000  34000.000000
25%    22.750000  37000.000000
50%    23.500000  39000.000000
75%    24.250000  40500.000000
max    25.000000  42000.000000

Data Info:
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 4 entries, 0 to 3
Data columns (total 3 columns):
 #   Column  Non-Null Count  Dtype 
---  ------  --------------  ----- 
 0   Name    4 non-null      object
 1   Age     4 non-null      int64 
 2   Salary  4 non-null      int64 
dtypes: int64(2), object(1)
memory usage: 228.0+ bytes
None
```

## Result
Thus, NumPy arithmetic operations and Pandas DataFrame operations were successfully performed. Descriptive statistical measures and dataset information were also obtained using Python libraries.
