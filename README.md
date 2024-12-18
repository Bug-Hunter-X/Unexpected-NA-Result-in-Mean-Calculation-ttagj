# Unexpected NA Result in Mean Calculation
This repository demonstrates a common yet subtle error in R when calculating the mean of a vector containing NA values. The default behavior of the `mean()` function is to return NA if any NA values are present, leading to unexpected results or disruptions in downstream analyses. The solution shows how to handle such situations gracefully.
## Bug
The provided R code calculates the mean of a vector that includes an NA value. The `mean()` function, by default, returns NA, masking the actual mean of the non-NA values.
## Solution
The solution introduces the `na.rm = TRUE` argument in the `mean()` function to explicitly remove NA values before calculating the mean. This ensures that the mean is calculated correctly, excluding NA values from the calculation.
