# Lung-Cancer-Detection-ResNet-50-
This code is written in Python and is used for building a deep learning model to classify lung cancer images using the ResNet50 architecture. Here is the analysis of the code:

    The first few lines are comments describing the environment, helpful packages, and the directory structure of the input data.

    The required packages are imported, such as numpy, pandas, tensorflow, keras, and so on.

    The image dataset is defined as "../input/lung-and-colon-cancer-histopathological-images/lung_colon_image_set/lung_image_sets".

    The size of the input image is set to 224 x 224.

    The ImageDataGenerator is used to prepare the training and validation dataset. The validation set is split into 20% of the total dataset.

    The ResNet50 architecture is used as a pre-trained model for feature extraction, and the final layers of ResNet50 are removed.

    Two fully connected layers with 256 and 128 neurons, respectively, are added on top of the ResNet50 architecture, followed by a final softmax layer with 3 neurons for classification.

    The model is compiled with 'categorical_crossentropy' loss function, 'adam' optimizer, and 'accuracy' as the evaluation metric.

    The training and validation loss is plotted using matplotlib. 

    Finally, the confusion matrix and classification report are generated to evaluate the performance of the model.

In summary, this code loads an image dataset, uses the ResNet50 architecture to extract features, and adds fully connected layers for classification. The model is trained and evaluated, and the results are presented using the confusion matrix and classification report.
