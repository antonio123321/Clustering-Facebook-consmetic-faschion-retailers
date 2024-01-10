- Thailand's Facebook Fashion and cosmetics 

This project aims to understand which types of posts effectively engage more customers when shopping online for fashion and cosmetics in Thailand using Facebook

DATASET
 The dataset include the following columns:
Status id
status type
Number of reactions
...

The libraries are imported

PART 1 DATA PREPROCESSING AND VISUALIZATION:
The data is visualized in particular the  categorical variable including post like: video photo.....

The column of no interest are taken off.

Data is encoded and a pairplot is generated.

Pca is used to reduce the dimensionality of the dataset

Data is standardized and the elbow method used to decide the right number of cluster to use when training the Kmeans algorithm

Grid search is used to get the right hyperparamethers for the Kmeans.

Part 2 Model training

K-means algoritm is trained and  evaluated, with results: 

silhouette score k-means  0.7349469324265064
davies bouldin score k-means 0.5314258511940954
calinsky score k-means 9514.59793388625

hyerachical clustering model is trained  and evaluated using the same data giving the results as:

siluette score hierarchical  0.732780621979845
David bouldin score hierarchical 0.5886941486211739
calinski_harabasz_score hierarchical 8485.322873083966

subsequently K-mean is chosen as algorithm to work with due to the best metrics.

Visualization of the clusters reveil that cluster one include mostly video and get the highest numberof engajements.
