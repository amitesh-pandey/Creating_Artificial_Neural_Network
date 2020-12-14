
"#Artificial_Neural_Network" 

In this repository we shall be creating a working Model for predicting whether the following customer will continue its account in the bank or else will leave the Bank. Here the dataset is very huge, I.e., almost 10,000 instances or in simple word we can say as, information of 10,000 customers and so applying Machine Learning Algorithm directly on such huge datasets leads to the complexity in the processing speed and might end up with hang of your computer system. </br>

So, in order to overcome this Limitation, there was a need to have a Model which can </br>
1. Extract the necessary features for a huge dataset by itself and perform the operations </br>
2. Work with the highly efficient when it comes to the high dimensional data’s </br>
3. Mimic the human’s brains to enhance the learning process of machines </br>

So here comes an introduction to Deep Learning and Neural Network concepts. </br>
Here we are working with the artificial Neural Network. An Artificial Neural Network is an information processing model that is inspired by the way biological nervous systems, such as the brain, process information. It has mainly three Layers: Input Layer, Hidden Layer, Output Layer. </br>
Talking about the flow of a code, the following steps taken in to consideration:</br>
1. Loading the dataset using Pandas Library </br>
2. Applying the Label Encoding and OneHotEncoding Techniques in order to replace the characters to numbers (As Artificial Brains Cannot Process the characters but only numbers)</br>
3. Using model_selection module in sklearn Library, splitting the huge dataset into training and testing dataset. The size of the testing dataset is kept on 0.2, I.e., 20% of number of instances and huge data are allocated in a training set, thus providing more opportunity for artificial brains to learn. </br>
4. Applying the feature scaling techniques in order to scale down the values in the same range defined </br>
5. Creating an artificial Neural Network using Tensorflow and Keras library. ReLu activation function is used in the input and hidden layers and sigmoid activation function is used in output layer. </br>
6. Finally compiling the model with the batch size of 32 for the 100 iteration or epochs </br>
7. I have received the accuracy levels of 86.33% on the training model and 85.99% on the testing model, which seems to be pretty good. </br>

Now question arises, </br> 
Question 1 : Why ReLu function in the hidden Layer? </br>
ANN uses the rectifier function for the hidden layers are referred to as rectified networks. As rectified linear units are nearly linear, they preserve many of the properties that make linear models easy to optimize with gradient-based method and so we don’t want the hidden layer to be non linear and create complexity in the networks. The hidden need to be simple, linear and optimized </br>

Question 2 : Why Sigmoid function in the Output Layer? </br>
The main reason why we use sigmoid function is because it exists between (0 to 1). Therefore, it is especially used for models where we have to predict the probability as an output. </br>
