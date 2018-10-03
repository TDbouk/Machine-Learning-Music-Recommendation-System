# Machine-Learning-Music-Recommendation-System
This is my Machine Learning Engineer Nanodegree capstone project. In this project, I have built a music recommendation system that recommendation system that recommends songs for users based on their music taste. The model works by clustering users with similar music taste and selects a random song from the clusters most listened to songs to keep users exploring new songs. 

Interested? Take a look at the [Notebook](music_recommender.ipynb). 

## Data Exploration
Explored the dataset composed of 1000 rows and 14 features using statistics and several visualizations such as Histogram, Scatter Matrix, and Heatmap to find trends and relationships within the data.

### Statistics
<img src="screenshots/data_stats.PNG" width="800">

### Histograms Exploring Males vs Females Music Taste
<img src="screenshots/barchart_songs_males.PNG" width="400" height="420"> <img src="screenshots/barchart_songs_females.PNG" width="450">

### Scatter Matrix Exploring Feature Relevance
<img src="screenshots/scatter_matrix.PNG" width="800">

### Heatmap Exploring Features Correlation
<img src="screenshots/heat_map.PNG" width="400">

## Data Preprocessing and Visualizations
Processed the data to identify suspected outliers using Tukey Method, visualized them, and evaluated their removal/presence impact.

### Box Plot to Visualize Data Distribution and Outliers
<img src="screenshots/box_plot.PNG" width="800">

### Swarm Plot to Visualize The Data Distribution in a More Focused Manner
<img src="screenshots/swarm_plot.PNG" width="800">

### Swarm/Box Plot to Analyze The Suspected Outliers
<img src="screenshots/box_swarm_plot.PNG" width="400">

## Dimensionality Reduction
Applied PCA to reduce data dimensionality to 3 dimensions and visualized features projections over the selected principal components that best explains the variance.

### Principle Components Analysis for Reducing Dimensions 
<img src="screenshots/pca_dimensions.PNG" width="800">

### PCA Cumulative Expected Variance
<img src="screenshots/pca_cumulative.PNG" width="400">

### PCA Feature Projection
<img src="screenshots/pca_plot.PNG" width="600">

## Clustering
Clustered the users using K-means by finding the optimal number of clusters using Silhouette score and created a newly engineered feature representing a user segment.

<img src="screenshots/graph_clusters.PNG" width="600">

## Model Evaluation
Built a Decision Tree Classifier that predicts the engineered feature (cluster label or user segment) and used it as a Gold Standard to evaluate several random and greedy benchmarks using F1-Score. The model is capable of predicting the newly engineered feature while achieving a 99% accuracy compared to 8% and 28% for the random and greedy benchmarks.
