### google AI crash course
### 手机安装linux终端Termux
* [如何安装jupyter notebook](https://github.com/ravish0007/AndroJupy/blob/master/README.md)
* 有些lib没有找到，
* [现有支持库](https://github.com/termux/termux-packages/tree/master/packages)
    * apache
    * nginx
    * git
    * python

[访问网址](http://192.168.31.188:8888/notebooks/ipynb/%E7%AC%AC%E4%B8%80%E6%AC%A1%E6%89%8B%E6%9C%BA%E8%BF%90%E8%A1%8Cjupyter.ipynb)
[初始网址](http://localhost:8888/?token=4aeab0593199bfb6dfa3ccc3f8450c6f9e35e7b93d2399d3)

```python
import matplotlib.pylab as pylab;
from math import sin, radians
pylab.figure(1)
R=range(360)
pylab.plot(\
[i for i in R],\
[sin(radians(i))for i in R])
​
print('ok')
```

```shell
#创建符号链接到我的文件夹
ln ~/storage/downloads/project/ ~/myproject --symbolic
$ ls -lhtr
total 16K
drwx------ 5 u0_a207 u0_a207 4.0K Dec  8 11:34 how-tomcat-works
drwx------ 2 u0_a207 u0_a207 4.0K Dec  8 15:36 storage
-rw------- 1 u0_a207 u0_a207   16 Dec  8 15:40 test.log
-rwx------ 1 u0_a207 u0_a207    9 Dec  8 15:43 exe.sh
lrwxrwxrwx 1 u0_a207 u0_a207   59 Dec  8 23:29 myproject -> /data/data/com.termux/files/home/storage/downloads/project/

[登陆ftp]
tcpsvd -vE 0.0.0.0 1024 ftpd -w /data/data/com.termux/files/home
```
[github配置ssh key](https://blog.csdn.net/u013778905/article/details/83501204)

### 语法
- [ ] test
- [x] test2
$\Gamma(n) = (n-1)!\quad\forall
n\in\mathbb N$

### 如何解决ML学习过程遇到的问题?
* 看大量书，好像懂了，但是没有实际操作还是不懂。
* 学习过程遇到大量生僻的专用术语，就应该像我们做项目的时候，遇到不懂的问题应该提出QA票，然后继续学。有时间再对应QA去一一突破。
* 学习实践首先带有一个好的工具IDE，达到事半功倍的效果
* 碎片化的时间学习。手机端放下游戏，安装IDE
* 还有关键的设立计划。工作中有WBS，学习也一样
* 时间和精力有限的情况下，All in AI。霍金年轻才华横溢毫无作为，但是生病后开始奋斗。上帝把所有门都关闭了，给开了一个窗户！
* 算法就是对某种问题的解决方案。
* 每个行业都有着自己约定俗成的一个流程。routine，熟悉后就不在神秘。就像魔法揭开谜底就没意思了
* 数学难学是因为教育过程中被抽象了。原来的数学是为了解决某个具体问题的。当年牛顿发明微积分是为了解决物理问题，而我们学习微积分是为了考试。
