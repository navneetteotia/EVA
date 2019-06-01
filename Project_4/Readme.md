# Architectural Basics

### Order of concepts:
1. Kernels and how do we decide the number of kernels?
>- **Kernels** are the feature extracters. Number of kernels depend on the data diension, objective of the exercise and granularity of the features. Complex features require more number of kernels than simple features.
2. 3x3 Convolutions
>- 3X3 Convolutions are useful in extracting complex features while keeping the total number of parameters low.
3. Receptive Field
>- **Receptive field** is the the space a convoulution pixel covers on the input image.
4. How many layers
>- Number of layers depends on the problem and dimensions of the input.
5. MaxPooling
>- **MaxPooling** extracts the most prominent feature from a layer.
6. Position of MaxPooling
>- MaxPooling is normally a part of transition layers, which is placed after 3-4 convoulution layers.
7. The distance of MaxPooling from Prediction
>- Since the features coming out of MaxPooling are too prominent, it is advised to have it 3-4 layers before the prediction.
8. 1x1 Convolutions
>- **1X1 convolutions** work in combining features from multiple channels into less, thereby helping in reducing the number of channels.
9. Learning Rate
>- **Learning rate** controls how much the weights in the network get adjusted towards the correct output.
10. Number of Epochs and when to increase them
>- Number of epochs must be increased in case the epochs run show a trend of moving towards better results.
11. Concept of Transition Layers
>- Transition layers are the layers between two blocks of convolution layers. They are used to reduce the dimension as well as number of channels, thereby using 1X1 convolution and MaxPooling.
12. Position of Transition Layer
>- Transition layers are placed between the convolution blocks.
13. How do we know our network is not going well, comparatively, very early
>- The state of network's performance is evident in the initial 4-5 epochs.
14. When to add validation checks
>- Always.
15. Image Normalization
>- Image Normalization is when the scale of every pixel in an image is adjusted to another scale based on the image itself. Eg: Changing the scale from 0-255 to 0-1.
16. SoftMax
>- **SoftMax** is the activation used in classification problems which provides a probability-like prediction.
17. Batch Size, and effects of batch size
>- Batch Size is the number of sample from the data that will be propagated through the network at a time. The batch size affects the training time and number of epochs it takes to reach an optimum accuracy.
18. Batch Normalization
>- Batch Normalization is where the images are normalized based on the entire batch of data.
19. The distance of Batch Normalization from Prediction
>- Batch Normalization must be at least 2-3 layers away from the prediction since it can affect the activations.
20. DropOut
>- DropOut is a way of regularization to reduce overfitting. It works by switching off a specified amount of parameters.
21. When do we introduce DropOut, or when do we know we have some overfitting
>- We introduce DropOut when the test accuracy is lower than the train accuracy and the difference between the two is high (overfitting).
22. Adam vs SGD
23. LR scheduler and concept behind it
>- Learning Rate Scheduler is used to decrease the learning rate systematically with time/number of epochs to converge faster. It is based on the concept that a higher learning rate in the beginning will take major steps towards the minima but the smaller learning rate later will help it not swing around the minima too long.
24. When do we stop convolutions and go ahead with a larger kernel or some other alternative
>- We stop adding convolutions when we have enough number of layers that can extract the features properly.
