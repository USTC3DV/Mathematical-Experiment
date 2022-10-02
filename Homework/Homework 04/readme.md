# Homework 04

## 内容如下：

- 从下述[数据集](https://vision.middlebury.edu/mview/)所提供的多视⻆图⽚数据，恢复物体的三维点云模型  
  - 数据集已提供了每张拍摄图⽚相机的内参，可以直接读取，具体惨⻅[数据说明文档](https://vision.middlebury.edu/mview/data/)；
  - 采⽤ [08_UncalibratedStereo.pdf](../PPT/08_UncalibratedStereo.pdf) 课件中的⽅法，每次以两张图⽚作为输⼊（某张图⽚固定）来恢复每个视⻆的点云，然后根据相机变换，将不同的视⻆的点云放在⼀个统⼀的坐标系下;
  - 需计算两张图⽚之间的相机变换，以及稠密点云恢复;