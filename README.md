Principal Component Analysis for Economic Indicators: Dimensionality Reduction and Data Visualization.

Objective:

This project focuses on applying Principal Component Analysis (PCA) to address challenges posed by high-dimensional economic indicator datasets. High-dimensional datasets, have numerous variables per observation, that can hinder analysis and interpretation. 

The primary goal is to simplify data interpretation, identify critical features, and visually represent data point relationships in a lower-dimensional space, thereby improving the comprehensibility and insights derived from complex economic datasets.

Motivation:

Understanding economic indicators is challenging due to their high-dimensional nature. We aim to simplify complex data by employing PCA, making it more accessible. This enhances the economics study and provides practical benefits, aiding policymakers, financial analysts, and decision-makers in gaining more precise insights into economic drivers.

Background:

People have used different methods to study economic indicators, especially when the data is complex. These methods involve using machine learning techniques such as clustering algorithms, regression models, and neural networks to find patterns.

Familiarizing with a few fundamental concepts is beneficial to grasp the project well. Firstly, having a good understanding of statistics, which involves analyzing data, will be helpful. Secondly, knowledge of specific math concepts like eigenvalues and eigenvectors will aid in comprehending the Principal Component Analysis (PCA) method used in the project. PCA is a technique that simplifies data by reducing its complexity while retaining essential information. In summary, possessing skills in statistics and a basic understanding of economics will enhance your ability to derive the most value from the project.

My Work:

Numerical Linear Algebra Methods used:

Standardization: Implemented StandardScaler from sci-kit-learn to standardize data, ensuring a mean of 0 and a standard deviation of 1 for each feature.
Covariance Matrix and Decomposition: Computed the covariance matrix and performed eigenvalue and eigenvector decomposition using NumPy.
Sorting and Selection of Principal Components: Identified influential features through sorting eigenvalues and eigenvectors.
Visualization: Employed Matplotlib for visualizing cumulative explained variance and scatter plots, enhancing data representation.

Project Implementation:

PCA Implementation: Successfully applied PCA to reduce dimensionality and transform the original dataset into principal components.
Cumulative Explained Variance: Calculated and visually represented cumulative explained variance, demonstrating that the first 15 principal components capture around 90% of the data's variation.
Color Mapping: The 'logan_passengers' column for color mapping in scatter plots provided additional information.
Interpretation: A clear and concise representation of economic indicators in a 2D space facilitates easier understanding.

Output Results Analysis:

Cumulative Explained Variance Graph:-

Cumulative explained variance is a measure of how much of the variation in the data is defined by the first few principal components. The graph indicates that the first 15 principal components capture approximately 90% of the data's variation. Beyond these components, the curve flattens, suggesting diminishing returns. The first two principal components are sufficient to capture essential information, reducing dimensionality.

Individual Explained Variance:-

The individual explained variance for the first two principal components in a dataset, which is reported as follows: Principal Component 1 accounts for 42.22% of the total variance, while Principal Component 2 explains 20.11%. These percentages represent the proportion of data variability captured by each principal component, providing insights into the significance and contribution of each component to the overall variance in the dataset.

Eigenvalue Contributions:-

The provided list represents each eigenvalue's contributions to a dataset's overall variance. Eigenvalue 1 has the highest contribution, accounting for 42.22% of the total variance, followed by Eigenvalue 2 with a contribution of 20.11%. Each subsequent eigenvalue contributes a decreasing percentage to the overall variance as the list progresses. The diminishing values indicate that the principal components associated with higher eigenvalues capture less variability in the dataset, highlighting the importance of the first few eigenvalues in explaining most of the data's variance. In contrast, the later ones have diminishing significance. This information is often crucial in dimensionality reduction techniques, such as principal component analysis, where the goal is to retain the most important features while discarding less relevant ones.

PCA Transformed Data Scatter Plot:-

From the graph, the data is probably high-dimensional, indicating numerous features. This is evident as a small number of principal components can account for a significant portion of the data's variability.

Additionally, the graph implies that the data is likely complex, indicating non-linear relationships between different features. This complexity arises because the relationship between components does not follow a straight line. The presence of noise, or random variation in the data, is noticeable as data points are scattered around the trend line.

Furthermore, the data contains outliers, signifying some data points significantly deviate from the overall pattern. This is apparent from a few data points far from the trend line.

Lastly, the data appears non-normally distributed, meaning its distribution is not bell-shaped. This is noticeable as data points are not evenly distributed around the trend line.

Conclusion:

We learn a few essential things from the above analysis about the dataset. First, we can simplify the data by focusing on the first 15 principal components, which capture the most important information (about 90%). This simplification helps us understand the data.

Looking at the details of Individual Explained Variance and Eigenvalue, we see that the initial ones are the most important in explaining what's happening in the dataset. This helps us decide which parts of the data are crucial and which are less important.

The scatter plot of the transformed data gives us a picture of how complex the data is. There are many features, and their relationships are not simple and straight. We also notice some points that stand out a lot from the rest, called outliers, and the data doesn't follow a typical bell-shaped curve, which might affect how we analyse it. In simpler terms, the data doesn't follow a normal distribution, meaning it's not evenly spread around an average. This is important because it suggests that standard statistical rules might not work well. Knowing this is crucial for picking the right ways to model the data and understanding how it might affect the accuracy of our statistical conclusions.

To sum it up, the PCA analysis of the dataset gives us a deep understanding. This understanding helps us make informed decisions about which features to use, how to optimize our models, and how to interpret the results. These decisions give us a strong starting point for further exploring the data and developing machine learning models.

References:

Data Source: Boston Economic Indicators
Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning. Springer.
Jolliffe, I. T. (2002). Principal Component Analysis. Springer.
Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., ... & Duchesnay, É. (2011). Scikit-learn: Machine learning in Python. Journal of Machine Learning Research, 12(Oct), 2825-2830.
