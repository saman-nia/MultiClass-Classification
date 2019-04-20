# Multi-Class Classification Features with Tensorflow an Scikit Learn Logistic Regression

# One vs. All: 

Here, you can see the performance of Deep Learning Vs. Machine Learning: <br />

![alt text](https://github.com/saman-nia/MultiClass-Classification/blob/master/data/Result.png) <br />

Here, you can see the performance of deep multi class classification: <br />

![alt text](https://github.com/saman-nia/Deep-Learning-MultiClass-Classification/blob/master/data/Image_Performance.png) <br />

Concept from: https://developers.google.com/machine-learning/crash-course/multi-class-neural-networks/one-vs-all <br />
One vs. all provides a way to leverage binary classification. Given a classification problem with N possible solutions, a one-vs.-all solution consists of N separate binary classifiers—one binary classifier for each possible outcome. During training, the model runs through a sequence of binary classifiers, training each to answer a separate classification question. For example, given a picture of a dog, five different recognizers might be trained, four seeing the image as a negative example (not a dog) and one seeing the image as a positive example (a dog). That is: <br />

Is this image an apple? No. <br />
Is this image a bear? No. <br />
Is this image candy? No. <br />
Is this image a dog? Yes. <br />
Is this image an egg? No. <br />

This approach is fairly reasonable when the total number of classes is small, but becomes increasingly inefficient as the number of classes rises. <br />

We can create a significantly more efficient one-vs.-all model with a deep neural network in which each output node represents a different class. The following figure suggests this approach: <br />

![alt text](https://developers.google.com/machine-learning/crash-course/images/OneVsAll.svg)



