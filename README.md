# speech-recognition
语音识别学习与练习

## Kaldi环境的安装
由于推荐使用Linux，因此在虚拟机下安装了环境，碰到两个问题
+ git克隆项目时最初是在windows环境下，然后将项目文件复制到虚拟机下，因此所有的脚本文件回车符为windows下的，在Linux下脚本不能正常运行
+ make项目时产生这样的错误g++: internal compiler error: Killed (program cc1plus)，百度后原来是内存不够，因此添加了内存，但是还是不行，因此教程中使用的4核make -j 4，改为make，之后的make过程中又出现了此问题，因此使用了网上开辟swap空间的方案，来源：`http://blog.csdn.net/fzh90/article/details/22893683`
