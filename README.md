# handwriting-recog
Data-Set
The dataset given to us is in the raw form. It contains 2 sets of datasets. 
1.	HUMAN OBSERVED FEATURES
2.	GSC OBSERVED FEATURES
Each of these datasets contains 3 files. 
1.	Raw data with features. Human observed data contains 1026 inputs with each input having 9 features. Whereas GSC dataset contains 14073 inputs with each input having 512 features.
2.	Each of these 2 datasets have additional 2 files. One of which has data about the ID of the images which have been written by the same writer/ author.
3.	Second file that corresponds to each of the 2 datasets has image IDs of 2 images written by different authors/writers.
The input for our training data shall be a pair of images and their features so that our model can learn to differentiate between images written by same writer and different writer. Hence we have thought of two types of solutions to the problem of feeding features of 2 images at once to our models:
1.	We can create new feature set by taking difference of respective features in the original data. 
•	In case of human observed data we will have a new set of features which will have same 9 features which are actually the difference between 2 similar or different images.
•	In case of GSC observed data we will similarly have 512 features.

2.	Secondly, we can also create new feature dataset by concatenating the features of the 2 images that will be compared in the model
•	In case of human observed data the new feature set will have 18 features.
•	In case of GSC observed dataset we will have similarly have 18 features.

# METHODS OF TRAINING
•	LINEAR REGRESSION MODEL FOR CLASSIFICATION.
•	LOGISTIC REGRESSION FOR CLASSIFICATION
•	NEURAL NETWORK
