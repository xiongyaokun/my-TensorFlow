# my-TensorFlow
learn something about ML with TensorFlow!

## Windows10下使用Anaconda安装TensorFlow
### 推荐使用pip3进行安装
<pre>
conda create -n my-tensorflow python=3.6
activate my-tensorflow
pip3 install --upgrade tensorflow
</pre>

### 普通CPU运行tensorflow可能出现如下错误：
'''python
2018-07-08 11:33:48.198427: I T:\src\github\tensorflow\tensorflow\core\platform\cpu_feature_guard.cc:140] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
'''
### 解决办法，在代码开始处：
'''python
import os
os.environ['TF\_CPP\_MIN\_LOG\_LEVEL'] = '2'
import tensorflow as tf
import numpy as np
'''
