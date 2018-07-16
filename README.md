# my-TensorFlow
learn something about ML with TensorFlow!
***
### [TensorFlow中文社区](http://www.tensorfly.cn/)
***
### [Sklearn与TensorFlow机器学习实用指南](https://mp.weixin.qq.com/s?__biz=MzI5NDY1MjQzNA==&mid=2247487162&idx=2&sn=86e178bfd0e419f831880fef60981207&chksm=ec5ed1c7db2958d1ba9c30adff9b3d1558203e24f3393297122307cb6df337bfe78f197867e6&mpshare=1&scene=1&srcid=07167KmQvFQCSCkMIr5xkeMB&pass_ticket=D0egOddlhmMa16%2BtzzB7nMTp3C05YZJvkdvwOeMSbKiWgvx3ockjprqA8T9ocEYQ#rd)

[Sklearn与TensorFlow机器学习实用指南-项目github](https://github.com/apachecn/hands_on_Ml_with_Sklearn_and_TF)  
[源码](https://github.com/ageron/handson-ml)
***
### [scikit-learn-doc-zh](https://github.com/apachecn/scikit-learn-doc-zh)
### [scikit-learn中文文档](http://sklearn.apachecn.org/)
### [sklearn-tutorial](https://github.com/jakevdp/sklearn_tutorial)
### [scikit-learn-examples](http://scikit-learn.org/stable/auto_examples/index.html#general-examples)
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
