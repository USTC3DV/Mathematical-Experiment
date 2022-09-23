### image stitching C++框架
**配置环境**：本次作业使用的是opencv4.5.5,且附带相同版本的opencv_contrib，通过cmake3.16编译。下载助教编译好的压缩包解压到任意路径（假设为D:\)，并在环境变量的系统变量的path里添加D:\OpenCV4\opencv4_build\install\x64\vc16\bin（注意！要添加在你们之前那个版本的opencv_build的上面，这样系统才会先在此版本的路径里找文件）
链接：https://rec.ustc.edu.cn/share/d82efc40-39cd-11ed-a1bf-c3ded61a1430

然后打开D:\OpenCV4\opencv4_build\OpenCV.sln，选择debug和x64
在解决方案资源管理器中，点击CMakeTargets，右击Install，选择生成。
然后换成release和x64，再生成一次。

之后打开群文件里下载的imagestitchingc++框架里的ConsoleApplication1.sln文件，就可以直接运行了。

#### 作业要求：

1. 用SIFT来进行特征检测，而不是框架里的SURF。
2. 要求能用5张或以上的图片合成全景图。

ps: 感兴趣的同学也可以自己用cmake编译opencv和opencv_contrib。