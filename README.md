# DataScience_Forum9
# Data Science Forum Week 9

# Unsupervised Machine Learning Algorithms and Evaluation
## Dataset: Diabetes Dataset
## Algorithms: KMeans Clustering, Mean shift clustering, Agglomerative Clustering, Spectral Clustering
## Evaluation methods: Silhoutte score, Davies-Bouldin index, Rand score, Calinski and Harabasz score

### 1. KMeans Clustering

  - <p align="justify">KMeans is a partitioning algorithm that divides the dataset into clusters.
    The number of clusters is first determined, which is K, and the dataset will be divided into K number of clusters. 
    The data points that are closest to the K randomly initialized centroids are continuously assigned to the cluster associated with that     centroid. The centroid is then computed using the recently allocated data point. 
    This procedure is repeated until the centroid's change falls below a predetermined threshold, indicating that it is sufficiently           stable (also known as convergence). The formation of the clusters occurs at this point.</p>
  - Results:
    - Silhouette Score: 0.603
    - Davies-Bouldin Index: 0.492
    - Rand Score: 0.014 
    - Calinski and Harabasz Score: 1719.56

### 2. Mean Shift Clustering

  - <p align="justify">MeanShift is a density-based algorithm that identifies clusters based on data density. Unlike KMeans, this algorithm
    doesn't need the number of clusters to be specified at the start (but it comes with a cost of the computing). Every data point is     shifted      
    toward the mean in its radius after mean shift clustering computes the mean of all the data points within a given radius for each data 
    point. Until convergence occurs, this process is repeated; the cluster centroid is then the data point that remained stationary 
    following convergence. Following that, the cluster centroids are assigned the data points.</p>
  - Results:
    - Silhouette Score: 0.585 
    - Davies-Bouldin Index: 0.505
    - Rand Score: 0.0146
    - Calinski and Harabasz Score: 1607 

### 3. Agglomerative Clustering

  - <p align="justify">Agglomerative Clustering is a hierarchical clustering algorithm that iteratively merges clusters. It starts by putting each observation
    into its own cluster. Eventually, there should only be one cluster remaining, which contains all of the observations. This will be achieved by repeatedly merging pairs of clusters that are closest to one another. The proximity between two clusters can be ascertained using a variety of factors.
    The hierarchy of clusters can be visualized as a dendrogram, which is a tree-like diagram that shows the order and distances at which clusters are merged.</p>
  - Results:
    - Silhouette Score: 0.544 
    - Davies-Bouldin Index: 0.479 
    - Rand Score: 0.010
    - Calinski and Harabasz Score: 1173.90 

### 4. Spectral Clustering

  - <p align="justify">Spectral Clustering employs the similarity matrix's eigenvectors to carry out clustering. Prior to clustering, the number of dimensions is decreased. It accomplishes this by computing the similarity matrix after first generating a similarity graph based on the similarity between data points. The similarity matrix's eigenvectors are then computed, and the resulting eigenvalues are utilized to create a new matrix. The data points are represented in a low-dimensional matrix as a result of this process, which decreases the dimension. Now that there are fewer dimensions, traditional clustering methods (like Kmeans) are used to perform the clustering process.
 
    
  - Results:
    - Silhouette Score: 0.370 
    - Davies-Bouldin Index: 0.380
    - Rand Score: 0.00021
    - Calinski and Harabasz Score: 17.904
  

### Findings:

  - Silhoutte score from best to worst: Kmeans > Mean shift > Agglomerative clustering > Spectral clustering

  - DBI from best to worst: Spectral clustering > Agglomerative clustering > Kmeans > Mean shift

  - Rand score from best to worst: Mean shift > Kmeans > Spectral clustering > Agglomerative clustering

  - Calinksi and Harabasz score from best to worst: Kmeans > Mean shift > Agglomerative clustering > Spectral clustering
    
