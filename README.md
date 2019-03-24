# Unsupervised Learning
## Project: K-means-Clustering-of-Movie-Ratings

### Install

This project requires **Python 3.6** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

### Run

In a terminal or command window, navigate to the top-level project directory (that contains this README) and run one of the following commands:

```bash
ipython notebook k-means Clustering of Movie Ratings.ipynb
```  
or
```bash
jupyter notebook k-means Clustering of Movie Ratings.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data

The data we'll be using comes from the wonderful [MovieLens](https://movielens.org/)[user rating data](https://grouplens.org/datasets/movielens/)

**Features**
- `mobieId`: Id for a movie
- `userId`: Id for an user
- `genres`: All the genres of a movie
- `title`: movie title
- `rating`: Rating given to the movie by the user
- `timestamp`: time when the user rated the movie 

### K mean clustering algorithm

- k-means is  one of  the simplest unsupervised  learning  algorithms  that  solve  the well  known clustering problem. 

- The procedure follows a simple and  easy  way  to classify a given data set  through a certain number of  clusters (assume k clusters) fixed apriori. 

- The  main  idea  is to define k centers, one for each cluster. 

- These centers  should  be placed in a cunning  way  because of  different  location  causes different  result. 

- So, the better  choice  is  to place them  as  much as possible  far away from each other. 

- The  next  step is to take each point belonging  to a  given data set and associate it to the nearest center. 

- When no point  is  pending,  the first step is completed and an early group age  is done. 

- At this point we need to re-calculate k new centroids as barycenter of  the clusters resulting from the previous step. 

- After we have these k new centroids, a new binding has to be done  between  the same data set points  and  the nearest new center. 

- A loop has been generated. As a result of  this loop we  may  notice that the k centers change their location step by step until no more changes  are done or  in  other words centers do not move any more. 

- Finally, this  algorithm  aims at  minimizing  an objective function know as squared error function given by:

![png](https://sites.google.com/site/dataclusteringalgorithms/_/rsrc/1273047853039/k-means-clustering-algorithm/kmeans.JPG)

where,

- ‘||xi - vj||’ is the Euclidean distance between xi and vj.
- ‘ci’ is the number of data points in ith cluster. 
- ‘c’ is the number of cluster centers.

In action:

![gif](https://github.com/shashank136/k-means-Clustering-of-Movie-Ratings/blob/master/image/kmean.gif)


##### Clusters of users who like romance and sci-fiction movies

![cluster Image](https://github.com/shashank136/k-means-Clustering-of-Movie-Ratings/blob/master/image/cluster.png)

- people who like romance but not scifi
- people who like scifi but not romance
- people who like both scifi and romance

##### Silhouette score representing similarity between a point and it's cluster

![png](https://github.com/shashank136/k-means-Clustering-of-Movie-Ratings/blob/master/image/silhouette.png)

##### Sunburn chart between most rated movies and users who rate movies the most for a cluster instance

![png](https://github.com/shashank136/k-means-Clustering-of-Movie-Ratings/blob/master/image/userplot.png)
