# Brain-Tumor-Detector
Machine Learning Model trained with K-Means Clustering and Color Segmentation to locate brain tumor. Kindly notice that this model is not perfect and should not be used for an actual clinic, this is simply a project I was practicing with. For almost perfect results I would recommend first consulting with a researcher/practicioner in the brain tumor area to be able to train the algorithm according to medical standards.

# What you can do
You would need to train the clustering algorithm on one Image, once you load the image make sure you flatten it and use the K-Means Clustering. After multiple tests I found that having 6 clusters produced the most efficient results but feel free to try a different number of clusters and compare results.

# After Training
Revert the clustered labels/results to the original unflattened shape and plot it, you will see different colors that vary depending on the cluster. Choose the cluster number which has the color that matches the tumor you can see and save the model.

# Testing
This is the tricky part now. So first you will have some images you'd like to test the model on. Loop through the images and find contours in each image to measure the area and we will decide whether the mass is a tumor or not based on that area ( This is one of the reasons that make consulting a practicioner important for production ).
Once the algorithm finds the area high enough to be considered a tumor, we will color the contours we found in yellow so user would see where the potential tumors are present.

# Tools used
Language / Environment: Python and Jupyter | 
Libraries: Scikit-Learn, Matplotlib, Opencv, Numpy |
Algorithms: K-Means Clustering
