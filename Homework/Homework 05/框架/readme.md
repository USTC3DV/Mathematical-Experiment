# 视频稳像（video stabilization）

方法来自论文[Bundled Camera Paths for Video Stabilization](https://github.com/USTC3DV/Mathematical-Experiment/blob/main/Homework/Homework%2005/%E6%A1%86%E6%9E%B6/Stabilization_SIGGRAPH13.pdf)。

- 视频稳像,是指利用相关的算法,对视频设备采集的原始视频序列进行处理,去除其中的抖动。

## 框架压缩包的内容：

- hw5：本次作业的框架，要求补充 `getPath.m`
- 论文：Bundled Camera Paths for Video Stabilization
- MeshWarpMatLab.zip：论文作者附上的代码，只有论文中的部分步骤
- ffmpeg：用以提取视频，合成视频
- example.mp4:示例视频

### 待处理视频：

可以使用示例视频作为待处理视频，也可以参照示例视频自己拍摄视频（必须为有晃动或视角转动之类不稳定情况的视频）。提交时，请将稳像后的新视频随代码和报告提交。如果是自己拍的视频，请将待处理视频也一并提交，以便对比处理前后效果。

### 运行方法：

1. 用 `ffmpeg` 提取待处理视频每帧，
   `ffmpeg -i example.mp4 image1/%03d.png` 
   （需要先创建文件夹 `image1`）

2. 运行 `run.m` 处理 `image1` 中的图像，存到另一个文件夹 `image2`

3. 用 `ffmpeg` 将 `image2` 中处理后的每帧合成为新视频
   `ffmpeg -i image2/%d.jpg output.mp4`

### 需要补充的代码：

- `getPath.m`中，依照论文中的方法，得到 `path` 的值
  提示：需要用到框架中的 `NewWarping` 函数和 `TrackLib.m` 中 `getF` 函数

#### `ffmpeg`安装：

- 解压 `ffmpeg-2022-10-10-git-f3b5277057-full_build.7z`，并选择 `Path` 变量，点击编辑按钮，在其原始内容后输入 `ffmpeg` 的 `bin` 路径。例如：`D:/ffmpeg-2022-10-10-git-f3b5277057-full_build/bin`
