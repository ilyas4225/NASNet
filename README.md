# Neural Architecture Search with NASNet

Here ['[NASNEt_Cifar10.ipynb'](https://github.com/ilyas4225/NASNet/blob/main/NASNEt_Cifar10.ipynb)] code loads the CIFAR-10 dataset and preprocesses the images by dividing the pixel values by 255 and one-hot encoding the labels. It then uses the NASNetMobile pre-trained model from the Keras library to build a new model by adding a GlobalAveragePooling2D layer followed by a Dense layer with 1024 units and a ReLU activation function, and finally a Dense layer with 10 units and a softmax activation function for classification.

The weights of the pre-trained layers are frozen, and the model is compiled using the Adam optimizer, categorical cross-entropy loss function, and accuracy as the evaluation metric.

The model is trained on the training set for 50 epochs with a batch size of 32, and the test set is used for validation during training. Finally, the model is evaluated on the test set, and the test loss and accuracy are printed.

Overall, this code uses transfer learning to build a model for image classification on the CIFAR-10 dataset and achieves a high accuracy on the test set.
