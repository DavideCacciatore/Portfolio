## **Conformal Predictions for Weather Image Classification**

In recent decades, Weather Recognition has become increasingly important, thanks to the growing
interest in Computer Vision and AI applications. Being able to analyze and classify visual conditions
at a given time and space has become necessary for many emerging sectors - just think of
the emerging world of autonomous driving assistance.

The recognition of weather conditions remains a not thoroughly studied subject, particularly when
it comes to the multi-labeling of weather and visual conditions, as they are often addressed individually.
The aim of this project is, therefore, to perform Weather Recognition; more precisely,
we try to predict to which of the chosen weather classes (*cloudy, foggy, rainy, snowy, sunny*) the
image belongs.

For this project, we used a **Python** kernel provided by *Google Colab* with an additional GPU for
the virtual machine. The main libraries used are numpy, sklearn and keras.

We exploited many methods and algorithms: as a first trial, we tried to classify our images using
classifiers as **Gaussian Naive Bayes**, **Random Forest**, **Logistic Regression** and **Support Vector Machines**
after appropriate pre-processing of the images. Then, we switched to **CNN** (Convolutional
Neural Network) and, subsequently, using the “feature extraction” part of the CNNs used, we used
the same classifiers as in the first part, noting a significant improvement in the results.

In this section, we added the **Conformal Predictions** as Interpretable Machine Learning task. The
weather images classification is a very complex problem, there are many situations were weather
conditions are unclear and cannot be identified in a single class. For this reason, we think that
Conformal Predictions can really help us describe an image.

As a benchmark model, we exploited **Efficient Net B4** to see how a pre-trained, and much more
complex, model would behave to solve our problem. This model is part of a class of pre-trained
models introduced by Google AI, specifically it is pre-trained on ImageNet and then applied to
the images in our train set.

Finally, we tested our models with their conformal predictions on a group of images taken directly
from us over the past few years to see their capability in real situations.
