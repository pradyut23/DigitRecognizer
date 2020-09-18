# DigitRecognizer
MNIST Digit Recognition.
The model uses an ensemble model with CNN layers for training.
Worked on this for my final year project, experimenting with different algorithms and hyperparameters, with this model as the final submission.

![MNIST](https://miro.medium.com/max/584/1*2lSjt9YKJn9sxK7DSeGDyw.jpeg)

# DATASET
The data files train.csv and test.csv contain gray-scale images of hand-drawn digits, from zero through nine.
Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.
The test data set, (test.csv), is the same as the training set, except that it does not contain the "label" column.

* Number of categories: 10
* Number of images: 4200 Training, 2800 Testing

The dataset can be found at: *https://www.kaggle.com/c/digit-recognizer/data*

# Training
The model uses an ensemble model with CNN layers.
The ensemble model runs for 10 iterations with each iteration consisting of Convolutional Layers, BatchNormalization Layers, MaxPooling Layers, Dropout Layers and Dense Layers.
The accuracy for the final model is averaged over all the 10 iterations.

Validation accuracy of **99.6%** is achieved for the final model.

# Conclusion
* The ensemble CNN model gives very high accuracy for this dataset.
* Most errors are recorded between the numbers 4 and 9.
