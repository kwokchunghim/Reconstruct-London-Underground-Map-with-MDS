# Reconstruct-London-Underground-Map-with-MDS

In this mini-project, we demonstrate a reconstruction of a London Underground map using a statistical technique called Multidimensional Scaling (MDS). 

MDS is essentially a dimensional reduction technique which is a generalisation of Principal Component Analysis (PCA) to arbitary dissimilarity matrices between point vectors. 

In usual PCA, the dissmilarity matrix usually coincides with Euclidean distances, but in this project, we used 'travelling time' between 2 stations to indicate how 'dissimilar' they are from each other.

The travelling time data between 10 London Underground stations were collected on 19th December 2022 from 18:45 - 19:15 (i.e. peak hours) based on Google Map route suggestions.

After constructing the dissimilarity matrix on a spreadsheet, we loaded the data into a Jupyter Notebook with Pandas and transformed it into a NumPy array. 

We then applied the MDS function in the Python Scikit-learn package and plotted the result with Matplotlib.

The result is interesting and in some ways, surpring. Despite that we are not trying to 'replicate' the original map, it is intuitive to compare our 'map' with the original London map.

We found that the MDS reconstruction correctly indicates the location of Heathrow and West Croyden, which happen to be further away from the rest of the 

References
[1] Kruskal, J. B., &amp; Wish, M. (2009). Multidimensional scaling. Newbury Park, Calif: Sage Publ.
[2] Sklearn.manifold.MDS. (n.d.). Retrieved December 21, 2022, from https://scikit-learn.org/stable/modules/generated/sklearn.manifold.MDS.html
