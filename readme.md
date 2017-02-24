# Description 
* The objective is to generate a number of adversarial examples of the number "2" from the MNIST database to fool a MNIST classifier to appear as "6"
* The project was started with some prior knowledge of NN such as perceptrons and MLPs
* First time dealing with CNNs and TensorFlow

# Progress completed
* Read through TensorFlow tutorial on building a CNN network
* Defined the parameters for convolution layers/pool layers 1 and 2
* Read through tutorial on dense/fully connected layer
* Read through tutorial on sessions and run-time analysis on tensorflow
* Build CNN with less than 2% error

# Things to do 
* Find a way to generate key pixel or data clusters that are associated with heavy weighting identifier of the number "6"
* Found paper which conceptualize the following solution:
  - Train the network using CNN
  - Save this network
  - Run the network through a test set of "2" images, during the session, introduce random "noise" or evolutionary steps for the image until the classifier thinks the image is a "6" (changes are kept if tf.matmul(h_fc1_drop, W_fc2) for 6 was increased from before)
  - Save this new image along with the old image in an isolated folder
  - Repeat this procedure 10 times

# Resources
* https://www.tensorflow.org/versions/master/tutorials/layers/
* https://www.researchgate.net/publication/283163432_HCNN_A_Neural_Network_Model_for_Combining_Local_and_Global_Features_Towards_Human-Like_Classification