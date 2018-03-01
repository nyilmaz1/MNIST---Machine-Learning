# MNIST---Machine-Learning
One of the projects I completed through a Udemy course called Machine Learning With TensorFlow is the MNIST or so called "Hello World" of ML. The dataset provides 28x28 images of handwritten digits (1 per image) and the goal is to write an algorithm that detects which digit is written. This is a classification problem with 10 classes. We will build a network with 2 hidden layers between inputs and outputs and try to make model predict what the given number is.   
I achieved 98% test accuracy by playing with the hyperparameters. I found the best combination is when the hidden layer size = 400; 2 hidden layers in total: learning rate = 0.001 with ReLu activation function in both layers. I could make the hidden layer size larger and learning rate more to increase the accuracy, but it takes too long to model to train. Following are my notes:  
##### hidden layer size = 50: test accuracy: 96.84  
##### hidden layer size = 200: test accuracy: 97.69 (longer time)   
##### hidden layer size = 400: test accuracy: 97.92 (takes much longer) 
##### hidden layer size = 200 + one more layer: test accur: 96.86   
##### hidden layer size = 200 + 5 hidden layers in  total: test accur: 96.91  
##### hidden layer size = 400 + 5 hidden layers in total: test accur: 97.14 (long)  
##### hidden layer size = 200 2 layers in total: with sigmoid in the last layer output (output_2): test accur: 97.58  
##### hidden layer size = 400 2 layers in total: with sigmoid " : test accur: 97.92  
##### hidden layer size = 400 2 layers in total: with softmax " : test accur: 70.21  
##### hidden layer size = 400 2 layers in total: with tanh " : test accur: 97.56  
##### hidden layer size = 400 2 layers in total: with softmax both outputs : test accur: 93.63 (started with low validation accuracy; took longer; more epochs; )
##### hidden layer size = 400 2 layers in total: with sigmoid both outputs : test accur: 97.82
##### hidden layer size = 400 2 layers in total: batch size = 1000: test accur: 97.73
##### hidden layer size = 400 2 layers in total: batch size = 1: test accur: (takes extra extra long)
##### hidden layer size = 400 2 layers in total: learning rate = 0.0001: test accur: (takes longer; more epoch) 97.88
##### hidden layer size = 400 2 layers in total: learning rate = 0.02: test accur: 94.46 (takes less time; less epochs)
##### hidden layer size = 400 2 layers in total: learning rate = 0.01: test accur: 96.49
##### hidden layer size = 600 2 layers in total: learning rate = 0.001: test accur: 97.81
##### hidden layer size = 400 2 layers in total: learning rate = 0.001: test accur: 98.02
##### hidden layer size = 400 2 layers in total: batch size = 500: test accur: 97.94
## hidden layer size = 400 2 layers in total: learning rate = 0.001: test accur: 98.17
