Colab Link to 7B: 

## Assignment 7A

### GoogLeNet incarnation of Inception Module:

![](https://github.com/navneetteotia/EVA/blob/master/Project_7/GoogleNet.JPG)

### Calcluation of Receptive Field of GoogLeNet incarnation of Inception Module:

 | Kernel Type | Kernel Size | Padding | Stride | Output | Jump | Receptive Field | 
 | --- | --- | --- | --- | --- | --- | --- | 
 | Convolution | 7 | 3 | 2 | 112 | 1 | 7 | 
 | Max Pooling | 3 | 1 | 2 | 56 | 2 | 11 | 
 | Convolution | 3 | 1 | 1 | 56 | 4 | 19 | 
 | Max Pooling | 3 | 1 | 2 | 28 | 4 | 27 | 
 | Convolution | 5 | 2 | 1 | 28 | 8 | 59 | 
 | Convolution | 5 | 2 | 1 | 28 | 8 | 91 | 
 | Max Pooling | 3 | 1 | 2 | 14 | 8 | 107 | 
 | Convolution | 5 | 2 | 1 | 14 | 16 | 171 | 
 | Convolution | 5 | 2 | 1 | 14 | 16 | 235 | 
 | Convolution | 5 | 2 | 1 | 14 | 16 | 299 | 
 | Convolution | 5 | 2 | 1 | 14 | 16 | 363 | 
 | Convolution | 5 | 2 | 1 | 14 | 16 | 427 | 
 | Max Pooling | 3 | 1 | 2 | 7 | 16 | 459 | 
 | Convolution | 5 | 2 | 1 | 7 | 32 | 587 | 
 | Convolution | 5 | 2 | 1 | 7 | 32 | 715 | 
 | Convolution | 7 | 0 | 1 | 1 | 32 | 907 | 
 
The inception modules have been assumed to have the receptive field of the branch that provides the highest receptive field. Among a 3X3 Convolution, a 5X5 Convolution and a 3X3 Max Pooling, 5X5 Convolution had the highest receptive field. 
