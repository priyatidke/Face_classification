# Face_classification
Problem Statement  : Face classification 

Human Face Classification

Total Images : 7601

Labels : 392

Model : Convolutional Neural Network

Accuracy on Train data : 98.70%

Accuracy on Test data : 95.97%
 
Parameter calculation:

1) The input_1(Input Layer) has shape (None,224,224,3) and parameter is 0.

2) stride = 3, kernel_size = 3 * 3, padding = same.

3) Convolutional_1 : ((kernel_size)stride+1)filters) = 3 * 3 * 3 + 1 * 32 = 896 parameters. In first layer, the convolutional layer has 32 filters.

4) Convolutional_2 : As convolutional_1 already learned 32 filters. So the number of trainable parameters in this layer is ((kernel_size)conv1filter(i.e.32)+1)filters) = 3 * 3 * 32 + 1 * 32 = 9248 parameters. In 2nd layer, the convolutional layer has 32 filters.

5) Convolutional_3 : ((kernel_size)conv2filter(i.e.32)+1)filters) = 3 * 3* 32 + 1 * 64 = 18496 parameters. In 3rd layer, the convolutional layer has 64 filters.

6) Convolutional_4 : ((kernel_size)conv3filter(i.e.64)+1)filters) = 3 * 3 * 64 + 1 * 64 = 36928 parameters. In 4th layer, the convolutional layer has 64 filters.

7) Convolutional_5 : ((kernel_size)conv4filter(i.e.64)+1)filters) = 3 * 3 * 64 + 1 * 64 = 36928 parameters. In 5th layer, the convolutional layer has 64 filters.

8) Convolutional_6 : ((kernel_size)conv5filter(i.e.64)+1)filters) = 3 * 3 * 64 + 1 * 64 = 36928 parameters. In 6th layer, the convolutional layer has 64 filters.

9) Dropout: Dropout layer does nothing. It just removes the nodes that are below the weights mentioned.

10) Max_pooling_2d: This layer is used to reduce the input image size.

11) dense_1: (43264 + 1) * 512 = 22151680

12) dense_2: (512 + 1) * 392 = 201096

11) At last all parameters sum together.(139424 + 22151680 + 201096). Total Training Parameter = 22,492,200 Trainable Parameters = 22,492,200 Non-Trainable Parameter = 0.
