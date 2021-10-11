# active-learning
A repository to store my experiments with active learning

Current Approach:
1. Train a CNN model on labelled cifar10 images
2. Use the trained model to make predictions on the unlabelled images of cats and dogs
3. If the most probable class as predicted by the trained network has low probability score, log the respective image to the weights and biases dashboard so that it can be labelled by humans and then added to the pool of training images.


## Possible Improvements
1. Instead of logging and labelling(by human) all images with low probability score, we can find out classes that the neural network is having trouble classifying using the confusion matrix and then only log images from those classes to the weights and biases dashboard to be labelled by humans.
