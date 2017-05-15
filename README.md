# Autonomous Learning: From Text to Vision
updated to Final Project
Details in (http://www.ee.columbia.edu/~cylin/course/bigdata/projects/)

## Description

The quick development of machine learning and deep learning in recent years enables data-driven artificial intelligence in various fields, including natural language processing, computer vision, speech recognition and data mining, to reduce manual work or support better decisions. However, most machine learning or deep learning applications that have been designed so far are established upon supervised machine learning, which requires a large set of annotated data as training set. Annotating a large amount of data could be extremely expensive, time consuming, and might be inconsistent if the annotators have different background or knowledge level. Thus, supervised machine learning methods are not able to implement the vast amount of unlabeled data in the world, and the results could be biased due to the limited resources of data. To solve this gap of knowledge and make full use of generally existing unlabeled data, autonomous learning, which implements statistical and unsupervised learning methods to achieve automated learning and predicting based on reference, rather than human interactions, has gradually attracted the attention of researchers and become a promising direction in artificial intelligence. 

In this project, we implement several unsupervised machine learning and deep learning methods to detect the category of objects in images by analyzing the images and corresponding captions. More specifically, we implement YOLO to detect objects, transfer learning to extract the feature representation of images and word embedding and GloVe to acquire the representation of words, and finally build a probabilisitc model to learn the label distribution and predict the categories of objects in images. 

Ideally, we feed the system with some raw images with text, the system can understand all the mapping relations. Later on, when we feed it with some other picture, it can tell us what kind of information such image conveyed. Or when we give the system some text, it can help us find some related cluster of pictures. 
If we feed the system with video, it can draw the bounding box and find out the cluster it belongs to.


## Deatils about code and demo:

### Configuration
To use this system, please ensure you have installed Tensorflow, Keras, and DarkNet (please refer tohttps://pjreddie.com/darknet/install/)
Some files in darknet need to be replaced with the files in "revise" folder to implement this system.
Make sure to configure DarkNet after the previous steps

Please refer to the deatils website to see the dataset used in this project.
Some codes in "additional" folder could be used to collect a valid dataset, such as scripting videos and captions from youtube, script images and captions in ms coco dataset, etc. 

### Code
please use the code in the following orders:
1. image_processing.ipynb


including object detection, feature extraction and clustering


2. text_processing_word_embedding.ipynb


used to compute word embedding as the word representation. If you intend to implement GloVe, please refer to https://nlp.stanford.edu/projects/glove/, where the code and pre-trained vectors are provided


3. label_inference.ipynb


compute the label distributions on captions, image clusters, and set the final score


4. video_processing.ipynb


a sample code to detect and reconstruct the video
a video demo is shown in https://youtu.be/vgkcREIa8Zg

