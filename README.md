# Experiments with Deep Neural Networks
In these Experiments used Python Language and Keras Library in Jupyter Notebook.
## Part 1: Training a deep feed forward network for multidimensional regression.
The **Feed forward neural network (FFNN)** model was created with the given polynomial equations, then train and validation data were prepared. 

The following steps were followed for model training:
1. Choose 𝑁 to be 1000. 
2. In your training data add some noise to 𝑦’s from a normal distribution with 𝜇 = 0.0 and 𝜎 = 0.001. 
3. Build a feed forward network with exactly 3 hidden layers.
 4. Define your loss function: o Use **MSE** for loss function. 
5. Train your algorithm with **SGD**. 
6. Repeat Steps 2-4 with another set of **activation functions** (3 different combinations), **learning rates** (3 different schemes) and **number of epochs** (after finding a reasonable number of epochs in the first trial, increase by 50% for 2 times). 
7. Choose your best parameters after Step 5. 
8. Add new nodes at a time to each hidden layer: 
- Start from the first hidden layer, add two nodes, train, and record results. 
- Move to the second hidden layer, add two nodes, train, and record results. 
- Move to the third hidden layer, add two nodes, train, and record results. 
9. Increase 𝑁 by 10% and repeat Step 8.

## Part 2: 2D Object Recognition using CNNs
The **2D-Shape-Generater** codes on Github were cloned, then images in different shapes were created with the functions in the repository. **(Oval, rectangle, triangle, poly 5, poly 6, poly 7, star 5, star 8)**.
These images were prepared as train and validation dataset, then a **Convolutional neural network (CNN)** model was created. 

The following steps were followed while creating the model:
1. Generate your data (online or offline) with 128x128 pixel images. Your data should have salt and pepper noise added in the images. Use only black-and-white colors.
2. Start with the **AlexNet model**. Change the input layer to handle grayscale images. Change the number of outputs to the right number of object classes. 
3. Use at least two different **learning rate** adjustment schemes and use at least three different **activation functions**. 
5. Change the **number of nodes** in the **fully connected layer** by 10% for three times and repeat Step 3. 
6. Continuing with %15 of the nodes in the fully connected layer, remove the third layer from the output and repeat Step 3. 
7. Continuing with %20 of the nodes in the fully connected layer, remove the third and fourth layers from the output and repeat Step 3.

