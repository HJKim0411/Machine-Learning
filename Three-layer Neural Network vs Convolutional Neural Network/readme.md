### Prior to entering...
- This project was made for comparison between 3NN and CNN.
- The basic CNN is a program provided by <https://goo.gl/VXK3hX> and I modified the CNN structure and data input for this experiment.
- Microsoft Visual Studio 2010 or later is required to use the program.
- In this system, you can train the 3-layer Neural Network and the Convolutional Neural Networks about training data. And you can test its performance about testing data. Also you can set the structure about each Neural Network.

### Examples of Input image
![input_image](http://i.imgur.com/yK8fXX3.jpg)  
- Input image size : 29x29.
- Data format : same with MNist data format.
- .nnt file(weights file) is different with MNist.

### About program
![system](http://i.imgur.com/ls7JODy.png)  
- Green box : The part that outputs the information in the neural network learning process.
- Purple box : The part that outputs the information of the test process.
- Black box : Buttons related to the nnt file (where the weight is stored).
- Brown box : Buttons related to data files to learn and test.
- Red box : The part that selects 3-layer neural network or convolutional neural network.
- Orange box : Button to start and stop learning.
- Blue box : Button to start and stop testing.
- If you click the button in red box, you can see the popup windows like belows.  
![popup](http://i.imgur.com/QYZb44z.jpg)  
In this windows, you can set the structure about neural network.  

### Result of experiments
##### 1. 3-layer neural network
- Number image, # of Training set : 498, # of Testing set : 153  
![1](http://i.imgur.com/ezKpHRX.jpg)  
- Number image, # of Training set : 498, # of Testing set : 153 + Contrast normalize  
![2](http://i.imgur.com/V7S5XGt.jpg)  
- Add background images  
![3](http://i.imgur.com/WuZRyfz.jpg)  
##### 2. Convolutional neural network
- Number image, # of Training set : 498, # of Testing set 153  
![4](http://i.imgur.com/ecYWFOX.jpg)  
- Add background images  
![5](http://i.imgur.com/1ji5gVn.jpg)  

### Conclusions
- For each situation, the number of hidden units should be adjusted.
- The larger the input size, the better the learning but the longer the learning time.
- Contrast normalization gives better learning effect.
- Convolutional neural network is better than 3-layer neural network.
- If the number of final outputs is large, the effect of learning decreases.
