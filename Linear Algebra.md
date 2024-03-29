# Linear algebra
## Principal Component Analysis (PCA):
 It is a dimensionality reduction technique used in machine learning and statistics to reduce the number of variables in a dataset while preserving most of its information.
 PCA aims to find a new set of variables (or principal components) that are linear combinations of the original variables. These new variables capture as much variance in the data as possible.
solving linear regression problems, image processing, recommendation systems.
 ### How PCA works?
#### Data Standardization:
PCA requires that the data be standardized, meaning that each feature should have a mean of 0 and a standard deviation of 1. 
This ensures that each feature contributes equally to the analysis.
##### explanation:
Data standardization, also known as data normalization, is a preprocessing step used to rescale the features of a dataset to have a mean of 0 and a standard deviation of 1.

Standard deviation is calculated as follows:
Calculate the mean of all data points. The mean is calculated by adding all the data points and dividing them by the number of data points.
Calculate the variance for each data point. The variance for each data point is calculated by subtracting the mean from the value of the data point.
Square the variance of each data point (from Step 2).
Sum of squared variance values (from Step 3).
Divide the sum of squared variance values (from Step 4) by the number of data points in the data set less 1.
Take the square root of the quotient (from Step 5).

-What Does a High Standard Deviation Mean?
A large standard deviation indicates that there is a lot of variance in the observed data around the mean. This indicates that the data observed is quite spread out.

Note for advanced readers – standardization (and studentization) assume that your data is normally distributed,

#### Covariance Matrix Computation:
PCA computes the covariance matrix of the standardized data. 
The covariance matrix shows the relationship between each pair of features in the dataset.

#### Eigenvalue Decomposition:
PCA then performs eigenvalue decomposition on the covariance matrix. This results in eigenvalues and eigenvectors. 
Eigenvectors represent the directions (or principal components) of maximum variance in the data, and eigenvalues represent the magnitude of variance along those directions.

#### Selecting Principal Components: 
The principal components are ranked based on their corresponding eigenvalues, with the first principal component having the largest eigenvalue, the second having the second-largest, and so on. Typically, only a subset of the principal components is selected to reduce the dimensionality of the data.

#### Dimensionality Reduction: 
Finally, PCA projects the original data onto the selected principal components, effectively reducing the dimensionality of the dataset. The new dataset consists of fewer variables (principal components) that capture most of the variance in the original data.
 
