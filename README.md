# my-TensorFlow
learn something about ML with TensorFlow!
***
### [TensorFlow中文社区](http://www.tensorfly.cn/)
***
### [Sklearn与TensorFlow机器学习实用指南](https://mp.weixin.qq.com/s?__biz=MzI5NDY1MjQzNA==&mid=2247486285&idx=3&sn=5e68ba944bed31644206902776ae36bc&chksm=ec5ed430db295d26db4117c1f263217d8621f86bf4bc72041d9ec50b810abee640c79c2d3535&scene=21#wechat_redirect)
[github](https://github.com/apachecn/hands_on_Ml_with_Sklearn_and_TF)
[源码](https://github.com/ageron/handson-ml)
***
## Windows10下使用Anaconda安装TensorFlow
### 推荐使用pip3进行安装
<pre>
conda create -n my-tensorflow python=3.6
activate my-tensorflow
pip3 install --upgrade tensorflow
</pre>

### 普通CPU运行tensorflow可能出现如下错误：
<pre>
2018-07-08 11:33:48.198427: I T:\src\github\tensorflow\tensorflow\core\platform\cpu_feature_guard.cc:140] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
</pre>
### 解决办法，在代码开始处：
<pre>
import os
os.environ['TF\_CPP\_MIN\_LOG\_LEVEL'] = '2'
import tensorflow as tf
import numpy as np
</pre>
