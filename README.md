# speech-recognition
语音识别学习与练习

## Kaldi环境的安装
由于推荐使用Linux，因此在虚拟机下安装了环境，碰到两个问题
+ git克隆项目时最初是在windows环境下，然后将项目文件复制到虚拟机下，因此所有的脚本文件回车符为windows下的，在Linux下脚本不能正常运行
+ make项目时产生这样的错误g++: internal compiler error: Killed (program cc1plus)，百度后原来是内存不够，因此添加了内存，但是还是不行，因此教程中使用的4核make -j 4，改为make，之后的make过程中又出现了此问题，因此使用了网上开辟swap空间的方案，来源：`http://blog.csdn.net/fzh90/article/details/22893683`

**一下午终于将Kaldi环境搭建好，不熟悉Linux的使用，使用的是虚拟环境，刚开始内存分配小了，make项目时出现错误，又改变分区，最后终于编译完项目**
## 学习Kaldi的最简单的测试例子yesno
</br>
</br>

## bash
**set -e 你写的每个脚本都应该在文件开头加上set -e,这句语句告诉bash如果任何语句的执行结果不是true则应该退出。这样的好处是防止错误像滚雪球般变大导致一个致命的错误，而这些错误本应该在之前就被处理掉。如果要增加可读性，可以使用set -o errexit，它的作用与set -e相同。来源`http://blog.csdn.net/todd911/article/details/9954961`**

**export 用于设置或显示环境变量。来源`http://www.runoob.com/linux/linux-comm-export.html`**

**head (head) 用来显示档案的开头至标准输出中。如果指定了多于一个文件，在每一段输出前会给出文件名作为文件头。如果不指定文件，或者文件为"-"，则从标准输入读取数据。`head (head) 用来显示档案的开头至标准输出中。如果指定了多于一个文件，在每一段输出前会给出文件名作为文件头。如果不指定文件，或者文件为"-"，则从标准输入读取数据。`**
