### Prior to entering...
- QFN : As a abbreviation for "Quad Flat No-leads Package" means that there is no lead part that is soldering part in SMD (Surface Mount Devices).
- QFN has many difficulties in soldering since there is no lead, and thus, many defects occur.
- Convolutional Neural Network with Color Input Images is used to inspect the defect of QFN.
- Dicing data and punch data were experimented.
- The basic CNN is a program provided by <https://goo.gl/VXK3hX> and I modified the CNN structure and data input for this experiment.
- Microsoft Visual Studio 2010 or later is required to use the program.
- OpenCV 2.4.9 is required, and environment variables should be added as follows:
Variable name : OpenCV, Value : opencv installation path\opencv\build


### Examples of Input image
- Image size : 29x29
- Original Color(RGB) images
![Input_images](http://i.imgur.com/jyTKH7G.jpg)

- Input image for one data (divide the above data into R, G, and B channels, respectively)
![Input_images2](http://i.imgur.com/vhpZO8N.jpg)

### About Convolutional Neural Network(CNN)
##### Common things with Neural Network
- One type of Multi-layer Neural Network
- Learning through backpropagation algorithm
##### Differences from General Neural Network
- Simple preprocessing recognizes visual patterns directly from pixel images
- Recognize highly variable patterns
- Robust to distortions and geometric changes in images
- Share Weight

### CNN structure used in experiments
![CNN](http://i.imgur.com/97K32Vx.jpg)

### Test results
- Experiment about Dicing data
![dicing_test_result](http://i.imgur.com/K3KQg3l.jpg)
-  Experiment about Punch data
![punch_test_result](http://i.imgur.com/TvGC0us.jpg)
