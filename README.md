# Multi-Class Classification Features with Tensorflow

# One vs. All: 
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
