#definition 
# K-Means Clustering

- most frequently used algorithm for [[Cluster]] data.
- starts by choosing _k_ random centers which you can set yourself.
	- step 0.: determine the ![[optimal number of clusters]]
- Then, all data points are assigned to the closest center based on their [[Euclidean distance]].
- Next, new centers are calculated and the data points are updated (see gif below). This process continuous until clusters do not change between iterations.

![](https://miro.medium.com/max/960/1*umzqxI8Oeje8nU5EItF5dw.gif)

_An animation demonstrating the inner workings of k-means — Courtesy: Mubaris NK_

Now in the example above the three cluster centers start very close to each other. This typically does not work well as it will have a harder time finding clusters. Instead, you can use _k-means++_ to improve the initialization of the centers. It starts with an initial center and makes sure that all subsequent centers are sufficiently far away. This optimizes the selection and creation of centers.