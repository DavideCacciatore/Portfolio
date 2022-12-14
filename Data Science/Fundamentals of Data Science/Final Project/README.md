## **SMS Spam Classification**

The purpose of this project is to build a model able to detect if a SMS is a spam message
or not. Many of our phones and sms apps have a spam detector that helps us to avoid
frauds, virus and malicious contents. We think this is an important topic and we wanted to
understand better how it works.

In our project we analyzed the [SMS Spam Collection Dataset](https://www.kaggle.com/uciml/sms-spam-collection-dataset) from Kaggle. This dataset
contains 5572 sms divided in two classes: ham and spam.

We pre-processed the messages, we divided the dataset in train and test set and then we
implemented the Naïve Bayes Model. In addition, we performed a cross validation analysis to
avoid considering only ham messages in our test set, because the dataset is unbalanced.
Then, we compared our best results with the metrics obtained by the most-voted notebook
in the Kaggle’s code section.

We also tried to change the default decision threshold and tried to use a Logistic Regression
model and compare our initial results with all this different setups. Finally, we saw what
are some of the mis-predicted sms in order to understand what could be the reasons of the
model’s mistakes.

For this project, we worked with Python and some of its libraries.

This project has been made with Simone Boesso, Giulio Corsetti, Francesca Possenti and Letizia Russo.
