## 配置要求：

- `Matlab` + `statistics and machine learning toolbox`
  - 如果你在安装 `Matlab` 时候**没有**安装所有工具包，那你需要补充安装上述工具包，只需在`主页->附加功能->获取附加功能` 里面直接搜索并安装即可（这是学校提供的正版软件可以做到的，盗版软件我就不知道了，正版软件可以在学校提供的[正版软件](http://ms.ustc.edu.cn/)里面直接下载并安装）；
  - 如果遇到其他工具包没有安装，只需参照如上安装即可；
- `MeshLab`：用于查看 $3D$ 点云文件
  - [官网](https://www.meshlab.net/)直接下载安装即可。

## ToDo：

需要补充代码的**只有`SFMedu2.m`、`estimateF.m`、`RTFromE.m` 三个文件**

- 不要畏惧这么大的框架，因为需要你干的工作已经很少了！！！
  - 你只需要先仔细阅读 `SFMedu2.m` 内各个模块的注释理解其含义，了解该系统的整个流程；
  - 再去逐步完成需要你实现的每个步骤即可；

- 完成 `SFMedu2.m` 中的第 45 行，计算内参矩阵；
- 实现 `SFMedu2.m`中`SIFT matching and Fundamental Matrix Estimation`模块内
  - `estimateF()`函数获取 Fundamental matrix，进而计算Essential Matrix；
  - `RTFromE()`函数计算第 $i$ 张图相对于第 $i-1$ 张图的 $[R|t]$；
- 实现 `SFMedu2.m`中`dense reconstruction`的模块内五个 `ToDo`，并思考这里一些步骤的原因；
- 默认运行 `SFM/images` 文件夹内的图片数据，所以如若需要运行其他图片模型，请修改：
  - `data`模块中 `17-21` 行数据读取；
  - `125、225`行的输出文件夹；



注：这是一个基本的 $SFM$ 系统的实现，感兴趣的同学可以自行了解相关其他模块的作用以及代码功能。