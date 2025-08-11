# Mean-Variance-Standard Deviation Calculator

This project consists of a single Python function that takes a list of 9 digits and uses the NumPy library to calculate various statistical measures on the resulting 3x3 matrix. This was completed as a requirement for the freeCodeCamp "Data Analysis with Python" certification.

## Function Overview

The `calculate()` function accepts a list of nine numbers. If the list does not contain exactly nine numbers, it raises a `ValueError`. Otherwise, it converts the list into a 3x3 NumPy array and computes the following statistics:

-   Mean
-   Variance
-   Standard Deviation
-   Maximum Value
-   Minimum Value
-   Sum

These calculations are performed along both axes (`axis=0` and `axis=1`) and on the flattened matrix.

The function returns a dictionary containing these results in a structured format.

### Example Output

For an input of `[0,1,2,3,4,5,6,7,8]`, the function returns:
```json
{
  "mean": [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  "variance": [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  "standard deviation": [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  "max": [,, 8],
  "min": [,, 0],
  "sum": [,, 36]
}
