# Myopia Clusters

## Description:
A medical research company believes that there might be distinct groups of patients that would be better to analyze separately in a data set being used to predict Myopia, or nearsightedness. Here I will explore this possibility using unsupervised learning. Starting with raw data, I will first prepare it to fit the machine learning models. Several clustering algorithms will be used to explore whether the patients can be placed into distinct groups. Following the models, I created a visualization to share my findings.

![myopia-illustration-330x220](https://user-images.githubusercontent.com/100361900/186709089-690ab99d-51a3-40fd-931c-8420c69fc9e4.gif)

## Process:

* Part 1: Prepare the Data
   * I prepared the data by removing the class column, checking for null values and duplicate rows. Lastly, I scaled the data for modeling. I saved the prepared data frame into a new csv for further anaysis separately if desired.

* Part 2: Apply Dimensionality Reduction 
   * I used PCA to preserve 90% of the explained variance, which reduced the number of features from 14 to 10. I then further reduced the dataset dimensions with t-SNE using the output of the PCA transformation so I could visually inspect the results with a scatter plot.

* Part 3: Perform a Cluster Analysis with K-means
   * I created an elbow plot to identify the best number of clusters, which is shown below. The elbow appears around K=5. 
   
<img width="479" alt="Elbow Curve" src="https://user-images.githubusercontent.com/100361900/186711037-85efa4a9-0c5e-4fa5-9b82-88610eff2845.png">

* Part 4: Make a Recommendation 
   * I used the K-means model to add a class column to the data set, then updated my scatter plot to color the clusters by class. It does appear that we could further analyze the data based on five groups of patients. The final plot is shown below.
   
<img width="430" alt="Clusters Plot" src="https://user-images.githubusercontent.com/100361900/186711078-30771574-058a-41a4-af22-34f5adbbdd34.png">


## Rubric

[Unit 20 Homework Rubric](https://docs.google.com/document/d/1046PZMnFwxcNkyIewuJc_RYhaErY42HoNUKORkh18A4/edit)

- - -

## References

Reduced dataset from [Orinda Longitudinal Study of Myopia conducted by the US National Eye Institute](https://clinicaltrials.gov/ct2/show/NCT00000169)

- - -

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.



