# yolov5p
Identify pedestrians, target and keep track of them     
识别行人、锁定特定目标并持续追踪。     
在我的另一个项目yolov5v6_pnnx的基础上加了一个基于ciou原理的小追踪算法。    
环境配置（arch linux）和代码编译都可以参考那个项目yolov5v6_pnnx。    
运行时直接调用摄像头0识别，识别过程中按q结束程序；按w开始/结束抓取；按e可以切换前一个识别目标，按r切换后一个。    
