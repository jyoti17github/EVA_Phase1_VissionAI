## Assignment_4(Architectural Basics):
Points are in order of our understanding of convolution neural network
1. ### Kernels and how do we decide the number of kernels?:
    Kernels are filter which convolves on input image and provide features for the next layer. The number of kernels are decided by the     size of input image. When we have more complex image we used to increase number of kernals.

2. ### Receptive Field: 
      It is the region of the input image where filter convolves.A dimension of RF is required to achieve before we apply hard operation        on layers 

3. ###  How many layers:
      Convolution layer, maxpooling layer, transition layer, fully connected layer, flatten layer

4. ###  3x3 Convolutions:
      3x3 is a three dimension vector which convolves on image to reduce dimension for the next layer by 2.This is very resource economic and have capability to reach any size of RF.

5. ###  ReLU:
      it is an activation function which turns negative weight to zero and pass all positive weight to next layer.It give major decision to extract useful informaton.

6. ### Batch Normalization:
        it puts the data set in range of 0 to 1 and deal with the problem of gradient explosion.This layer we use to apply after convolution operation.It does useful to improve model performance.

7. ### The distance of Batch Normalization from Prediction:
        Batch normalization should be used before prediction.

8. ### DropOut:
          It ignores neurons during training of certain set of neurons which is chosen at random. Ignored neurons do not consider by      DropOut layer during forward or backward propagation and this will help model to learn more and improve performance of model.

9. ### Image Normalization: 
        It is used to increase contrast of the pixels for effectively extraction of features and this help to increase effectiveness of Model

10. ###  MaxPooling: 
        it reduces the dimensionality of feature map into half size of image which creates a condensed feature map useful for passing the high weighted feature to next layers.

11. ### Position of MaxPooling:
          MaxPooling should be used after at least three or four convolution layers.

12. ### The distance of MaxPooling from Prediction:
          MaxPooling is used before 3 or 2 layers before prediction.

13. ### Concept of Transition Layers:
          Transition layers are such layers in convolution block where depth of feature maps remain constant but number of channel could be changed in this block.

14. ### Position of Transition Layer:
            It should be used after MaxPooling layer in convolution block.

15. ### 1x1 Convolutions:
            1x1 is merging the pre-existing feature extractors, creating new ones, keeping in mind that those features are found together.It help in combine related feature togeter.

16. ###  When do we stop convolutions and go ahead with a larger kernel or some other alternative (which we have not yet covered):
             When image is very complex we do need more kernals to extarct features.We stop convolution before flatten layer.

17. ###  Adam vs SGD: 
         Overall Adam is used as default optimizer and perform good with less complex dataset.Adam computes individual learning rates for         different parameters. Adam combines the advantages of two SGD extensions — Root Mean Square Propagation (RMSProp) and Adaptive           Gradient Algorithm (AdaGrad). SGD only computes on a small subset or random selection of data examples. SGD produces the same           performance as regular gradient descent when the learning rate is low.

18. ###  SoftMax:
         it is an activation function which converts output of the last layer based on probability distribution. And generate the single output.

19. ### When do we introduce DropOut, or when do we know we have some overfitting:
         When Test or Training accuracy is higher than validation accuracy it is said to be overfitting.When we see overfitting dropout can be use with proper parameter values i.e. less at beginiing layers and more in mid layers.

20. ### Learning Rate: 
          It is a hyperparameter to tune our network model for better performance. it is also called step size which adjusted weights for         each step during training. it's value is between 0.0 to 1.0. Learning rate usually help when model is not performing well after applying all important layer concepts and Training accuracy not reached to maximum value point.

21. ###  LR schedule and concept behind it:
           LR schedule is also called Addaptive LR. It systematically drops the learning rate at specific times during training network.           Example- suppose we have initial learning rate Lr1 drops it by Lr2 every n epochs. It help in improving accuracy and passing local minimas.

22. ### How do we know our network is not going well, comparatively, very early:
          In first 10 epochs if training and Validation accuracy not increasing in sync.Normally We check first twoor three epoch output validation accuracy to know about the efficiency of our network.

23. ###  Batch Size, and effects of batch size:
           Batch size is a set of samples of training data that used in iteration of each epoch. Bigger batch size quicken the iteration           process in each epoch and vice versa.With more batch size network can learn faster per epochs.

24. ### Number of Epochs and when to increase them: 
          one epoch is the complete processing of training data through designed network. To increase our validation accuracy we increase         number of epochs.
25. ### Checkboard Issue:
          when we convolve with a stride of more than 1, we would be covering some pixels more than once and creating island of extra             information spread around in a repeating pattern. 

26. ### Activation function:
          Activation function is used to fire neuron if information receiving by neuron is relevant for the information given. They are           required to do non-linear transformation
27. ### Validation Check : To check our network is performing good with respect to validation data set. we evaluate our model on Validation dataset.