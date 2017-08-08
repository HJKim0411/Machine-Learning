### 들어가기에 앞서...
  
- QFN : Quad Flat No-leads Package의 약자로써 SMD(Surface Mount Devices)중에서 납땜을 하는 부분인 리드가 없는 것을 의미함
- QFN은 리드가 없기 때문에 납땜을 하는데 있어서 많은 어려움이 있고, 이에 따라 많은 불량이 발생하고 있다.
- QFN의 불량 검사를 위해 컬러 입력 영상을 Input으로 하는 Convolutional Neural Network를 사용함
- QFN의 여러 종류 중  Dicing과 Punch에 대하여 실험
  
### 입력 영상 예시
  
- 영상 크기 : 29x29
- 원본 컬러(RGB) 영상
![](Input_images.jpg?0.9069261343771158 )  
  
- 하나의 데이터에 대한 입력 영상(위의 데이터를 R, G, B 채널로 각각 나눔)
![](Input_images2.jpg?0.9520490342285279 )  
  