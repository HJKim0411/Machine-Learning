### Prior to entering...
- This project is a project to detect defect beans in coffee beans.
- Nowadays, there are many places where experts inspect defective beans by hand.
- This work takes a long time and we have been working on this project to solve this problem.
- The basic CNN is a program provided by <https://goo.gl/VXK3hX> and I modified the CNN structure and data input for this experiment.
- Microsoft Visual Studio 2010 or later is required to use the program.
- OpenCV 2.4.9 is required, and environment variables should be added as follows:
Variable name : OpenCV, Value : opencv installation path\opencv\build
- In this system, you can make training datas from the image. And you can train the Convolutional Neural Networks about this training data. Also you can adjust the simple camera setting. Finally, you can detect the defect beans.

### Types of Defective Bean
- There are two types of defects covered in this system.
- The defect about shape(broken)    
![broken](http://i.imgur.com/WdpFaGC.jpg)  

- The defect about Insect Damage  
![Insect_damage](http://i.imgur.com/Gv38MLn.jpg)  
It can be seen that a dark hole was drilled in the part where the defect about Insect damage.  
(Image source : <http://www.coffeeresearch.org/coffee/defects.htm>)  

### Examples of Input image
- Original image  
![original](http://i.imgur.com/v2FNi4B.png)
- Shape Data  
 ![Shape_data](http://i.imgur.com/1Lgo3MP.jpg)  
 This is a resize of a 110x110 original image captured by Blob Labeling to 28x28. In order to prevent CNN from being influenced by the angle of the bean, I rotated the bean by 10 degrees to make the data.(36 data for one bean)  
- Insect Damage Data  
![Hole_data](http://i.imgur.com/0WCU45x.jpg)  
This data is a 28x28 crop around the darkest pixel in the 110x110 Original Image. (If you use the whole of the bean like the shape data, the effect is not good and the detection is difficult.)


### Applied to CNN(Convolutional Neural Network)
- In this system, I constructed two CNNs to deal with two defects.
- CNN for detecting shape defect(Shaped Neural Network)
- CNN for detecting insect damage(Insect Damage Neural Network)
- The system flow chart is as follows.  
![System_Flowchart](http://i.imgur.com/zB2zUkE.jpg)  

### Examples of result
- The red line boxes are results of defect.  
![result](http://i.imgur.com/IiU720Z.png)
