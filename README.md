# Neural-network-from-scratch

Created a neural network completely from scratch using only python and numpy and trained it on a small scaled custom made dataset. Also trained a sequential single layered neural network with the same parameters and achieved almost identical results.

The dataset contains 3 features : Age, Affordability, and Bought_insurance

## Custom Neural Network implementation and parameters
### Activation function : Sigmoid
As we have to do a binary prediction of whether someon bought insurance or not, sigmoid is an ideal choice.
![Sigmoid](NN_static/sigmoid.png)
![Formula](NN_static/sigmoid2.png)
### Loss function : Binary_crossentropy / Log loss
For classification models predicting the probability, the loss function most commonly used is cross entropy.
![Loss](NN_static/log_loss.png)
### Gradient Descent
initialized the weights(w1,w2) with 1 , bias with 0, and learning rate with 0.5

For each epoch a weighted sum is calculated -> w1 * Age + w2 * Affordability

Converted into predictions -> Sigmoid(weighted_sum)

Calculates loss -> Log_loss(y_true, y_predicted)

Re-adjusting weights and biases using the following formula : 
