### 本次作业为image stitching，运行方法：

1. 在data文件夹里创建文件夹 （eg：images），把你要拼接的图像放入images。

2. 将你的图像重命名为1.jpg，2.jpg，3.jpg。。。。。

3. 在工作台中输入
   im_out=Main(images,num_im,1);
   其中images是文件夹名，num_im是你的图片数量，1为显示拼接结果。

### 需要补充的代码：

1. 在函数get_put_matches.m里通过仿照hori(horizon)填写verti(vertical)。

2. 在函数get_T_for_all.m里计算每张图片对应已选定的中心图片的transform matrix。

3. 改写get_stitchM达到blending images 而不是简单拼接。



