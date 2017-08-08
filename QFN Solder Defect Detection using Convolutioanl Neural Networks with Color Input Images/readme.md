### 들어가기에 앞서...
- QFN : Quad Flat No-leads Package의 약자로써 SMD(Surface Mount Devices)중에서 납땜을 하는 부분인 리드가 없는 것을 의미함
- QFN은 리드가 없기 때문에 납땜을 하는데 있어서 많은 어려움이 있고, 이에 따라 많은 불량이 발생하고 있다.
- QFN의 불량 검사를 위해 컬러 입력 영상을 Input으로 하는 Convolutional Neural Network를 사용함
- QFN의 여러 종류 중  Dicing과 Punch에 대하여 실험

### 입력 영상 예시
- 영상 크기 : 29x29
- 원본 컬러(RGB) 영상
![Input_images](http://i.imgur.com/jyTKH7G.jpg)

- 하나의 데이터에 대한 입력 영상(위의 데이터를 R, G, B 채널로 각각 나눔)
![Input_images2](http://i.imgur.com/vhpZO8N.jpg)

### CNN 소개
##### 일반 Neural Network와의 공통점
- Multi-layer Neural Network의 한 종류
- Backpropagation algorithm을 통한 학습
##### 일반 Neural Network와의 차이점
- 간단한 전처리를 통해 픽셀 이미지로부터 곧바로 시각적 패턴을 인식
- 가변성이 큰 패턴 인식 가능
- 영상의 찌그러뜨림이나 기하학적인 변화에 강건
- Weight(가중치)를 공유
- Spatial topology를 잘 잡음

### 실험에 쓰인 CNN 구조
![CNN](http://i.imgur.com/97K32Vx.jpg)

### 테스트 결과
- Dicing 데이터에 대한 실험
![dicing_test_result](http://i.imgur.com/K3KQg3l.jpg)
- Punch 데이터에 대한 실험
![punch_test_result](http://i.imgur.com/TvGC0us.jpg)
