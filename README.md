# From-Text-to-Vision
updated to milestone 3

The 'Bounding Box Prediction & Clustering' file is used to do the image process. 
1. It uses the transfer learning method based on ResNet50 to develop a 4 output regressive model to predict the bounding box. 
This model can also be used to predictthe catagory of that bounding box object.
2. We crop the picture according to the bounding box we predict
3. We extract the feature of the cropped bounding box image and clustering them into 85 catagories
