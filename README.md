# Early_Stopping_using_Neptune.ai
Early stopping using PyTorch and Neptune for CIFAR10 Image Classification dataset

![Pytorch_logo](https://user-images.githubusercontent.com/69073063/111981222-adb0a900-8b07-11eb-9df0-cae951b36563.png)

![neptune-logo](https://user-images.githubusercontent.com/69073063/111981252-b6a17a80-8b07-11eb-93c7-d65fd136a030.png)

Early Stopping in Neural networks

One of the major challenges in training neural networks is how long to train the neural network. 
Training the model for a limited number of epochs can lead to underfitting and training the model for high numbers of epochs can lead to overfitting. 
Hence, it is very important to monitor the training process to stop the training at an appropriate time. 

In this experiment, we will discover that stopping the training of neural networks early before it overfits, 
can actually reduce overfitting and will lead to better model performance not only on the training dataset but also on the testing dataset. 

During the training of the neural network, there will be a point when the model will stop generalizing and start learning the noise in the data, 
which makes the model perform poorly on the unobserved data. In order to overcome this issue, we will use the number of epochs as one of the hyperparameters and monitor the training, and the testing loss. 

During the training of the neural network, we will feed the testing dataset after every epoch and monitor the testing loss, 
if the model performance degrades or in other sense, the testing loss starts to increase and accuracy decreases, the training process will be stopped. 

![early stopping](https://user-images.githubusercontent.com/69073063/111980655-e734e480-8b06-11eb-89f9-068e4af1cc3b.png)

Experiment is performed using PyTorch and Neptune.ai on CIFAR10 Image classification dataset using Convoltion Neural Netowork.

Results without Early Stopping

![Results](https://user-images.githubusercontent.com/69073063/111980980-54487a00-8b07-11eb-8c53-0afd6fc9ebf0.png)

Results with Early Stopping and patience value 10

![Untitled picture](https://user-images.githubusercontent.com/69073063/111981531-1861e480-8b08-11eb-9ade-8014cd625a1e.png)

![Results_2](https://user-images.githubusercontent.com/69073063/111981108-8063fb00-8b07-11eb-95d4-a0576cbb71cf.png)


