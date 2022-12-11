# Face-Recognition-and-Classifier
Recognize faces from a folder of images and classifies images if common person is found


This code uses the OpenCV library to detect faces in images. It creates a face cascade object using a pre-trained Haar cascade classifier, which is a machine learning algorithm that can be used to detect objects in images. The code then iterates over the images in a specified folder and detects faces in each image using the cascade object. If any faces are detected, the code draws a rectangle around them and displays the image.

1. The code imports the necessary libraries, including OpenCV and NumPy.
2. It loads the cascade classifier for face detection, which is a pre-trained machine learning model that can be used to detect faces in images.
3. It also loads a face recognition model, which is another machine learning model that can be used to recognize and classify faces in images.
4. The code then reads the images in a specified folder and converts them to grayscale, as this is required by the face detection and recognition models.
5. Next, the code detects faces in each image using the cascade classifier and adds them to the training set for the face recognition model.
6. It then trains the face recognition model on the training set, which allows the model to learn to recognize and classify the faces in the images.
7. The code then uses the trained face recognition model to predict the labels of the faces in each image.
8. It groups the images by the predicted labels, which allows it to group together images that contain the same person.
9. Finally, the code prints the number of groups and displays the images in each group.
10. At the end the code creates a new folder for each group of images, using the predicted label of the faces in the group as the name of the folder. It then saves the images in each group to the corresponding folder. This allows the code to organize the images into separate folders based on the faces they contain.

**NOTES**
1. I use haarcascade_frontal_face_classifier.xml  you can make your own classifier with tools like cascade trainer and crop a bunch of positive and negative images to make a cascade.xml file and run that through.
2. Make a folder of images in the main directory which need classification.
3. The output should be another folder containing all the face groups.


**TODO**
1. Move original images to said groups
2. Check the accuracy in larger data sets
3. Convert the greyscale image tags as icons for the folders
