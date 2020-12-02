# Self-Supervised MNIST Classifier with Autoencoders
### Autoencoder
The autoencoder is a **self-supervised** artificial neural network that learns how to compress and encode data then learns how to reconstruct the data back from the reduced encoded representation to a representation that is as close to the original input as possible.
#### Encoder
The encoder compressed the 28x28 MNIST image into a **feature vectors**. These will be used for the clustering task.
#### Decoder 
The decoder **reconstructs the input** based on the compressed representations of the given images.

### K-Means
The K-means algorithm groups similar data points into *k* clusters based on the arithmetic mean or **centroid** nearest to it. The objective function is defined as:

![K-Means Objective Function] (https://www.saedsayad.com/images/Clustering_kmeans_c.pngLarge)

### Hungarian Algorithm
The Hungarian Algorithm efficiently assigns labels to each cluster. It involves subtracting the **row minima** then the **column minima** from each row and column respectively. A minimum number of horizontal and vertical lines must be drawn over rows and columns with **0 entries**. An optimal assignment can be found if there are *n* lines required. Otherwise, the smallest uncovered element is subtracted from all the other uncovered elects and added to the covered ones.
