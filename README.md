<p align="center">
  <img src="./clustering.png" alt="Description of image" width="300">
</p>


# DTSA 5510 - Unsupervised Algorithms in Machine Learning Final Project


## Project Overview : Unsupervised Clustering on Tabular Data
This project tackles an unsupervised clustering task, where the goal is to predict clusters for a given dataset without any prior labels or information about the number of clusters. The project uses several clustering algorithms to classify the data and evaluates them based on the Adjusted Rand Index.

# Approach
The project follows a structured approach to analyzing the dataset and selecting suitable clustering models:

* Exploratory Data Analysis (EDA):

  * The initial EDA includes loading the dataset, handling missing values, and examining the distribution of discrete and continuous features.
  * Visualizations are used to explore feature distributions and identify any anomalies or patterns that could inform model selection and preprocessing steps.
* Preprocessing:

  * Scaling and Transformation: Features are transformed using a power transformation to ensure uniform scaling across columns, improving clustering performance.
  * Feature Selection: Some features that show little variation across clusters are removed to streamline the clustering process, based on insights from the EDA and visualizations of cluster centers.
* Clustering Models:

  * K-Means: Used as a baseline clustering algorithm, tested across a range of cluster numbers to find the optimal setup using the Elbow method.
  * Gaussian Mixture Model (GMM): This model allows clusters to take on various shapes, improving performance in scenarios where clusters are not spherical.
  * Bayesian Gaussian Mixture Model (BGMM): The best-performing model in this project, offering flexibility in the number of clusters by incorporating prior distributions over cluster parameters.
* Evaluation:

  * The models are evaluated using the Adjusted Rand Index (ARI), a measure of similarity between the predicted and true clusters.
  * Feature Importance: Analyzes which features contribute most to cluster differentiation, potentially guiding future feature engineering efforts.
* Results and Future Work
  * Model Performance: The Bayesian Gaussian Mixture Model (BGMM) achieved the highest ARI score among the tested models, indicating its effectiveness in capturing the data’s underlying structure.
  * Next Steps:
    * Further exploration with custom algorithms, such as Expectation Maximization (EM), could potentially improve clustering performance.
    * Applying statistical tests to understand feature distributions in more detail, which might inform additional feature selection and engineering strategies.
# References

* [Tabular Playground Series- Jul 2022](https://www.kaggle.com/competitions/tabular-playground-series-jul-2022)
