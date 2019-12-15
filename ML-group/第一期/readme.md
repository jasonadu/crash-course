### 第1课 音乐推荐系统_(上)
#### 1. 大纲
* 第一期：[【机器学习项目】第1课 音乐推荐系统_(上)](https://www.bilibili.com/video/av54736297?from=search&seid=17890613965883443557)  
  * 来源：[七月在线 机器学习项目班](https://www.julyedu.com/course/getdetail/48/)
  * 分享者：Jason
  * 时间：12月19日
  * [课件与代码](https://share.weiyun.com/5GkwBgK) oisaxl
  * 整理QA
    * 什么是推荐系统 
      * 快速参考 
        * [麦子学院人工智能教程](https://www.bilibili.com/video/av70039845) P98第02阶段：机器学习经典算法_11推荐系统
          1. python数据分析与建模
          2. 经典算法
          3. 案例实战
        * [补足 Surprise简介](https://www.bilibili.com/video/av37644716?p=7)
    * 涉及的算法
    * 项目如何进行
      * 数据收集 -> 数据清洗 -> 在训练集预估模型 -> 在测试集验证 -> 根据结果调整参数

#### 2. 什么是推荐系统

#### 3. 涉及的算法

#### 4. 项目如何进行

##### 安装[Surprise](http://surprise.readthedocs.io/en/stable/index.html)

运行Anacoda Prompt，输入

```
pip install surprise
```

**需要C++ Runtime**

* 安装问题1. SSL certificate

```
(base) C:\Users\Administrator>pip install surprise
Collecting surprise
  Could not fetch URL https://pypi.python.org/simple/surprise/: There was a prob
lem confirming the ssl certificate: [SSL: CERTIFICATE_VERIFY_FAILED] certificate
 verify failed (_ssl.c:645) - skipping
  Could not find a version that satisfies the requirement surprise (from version
s: )
No matching distribution found for surprise

# 添加信任，也没有解决
pip --trusted-host pypi.python.org install surprise
```

一路挫折：[surprise](https://pypi.org/project/surprise/) -> [scikit-surprise](https://pypi.org/project/scikit-surprise/#files)  -> pip install failed -> [install from file](https://packaging.python.org/tutorials/installing-packages/)

```
(base) C:\Users\Administrator>pip install D:\download\scikit-surprise-1.1.0.tar.
gz
Processing d:\download\scikit-surprise-1.1.0.tar.gz
Requirement already satisfied: joblib>=0.11 in d:\tools\anaconda3\lib\site-packa
ges (from scikit-surprise==1.1.0) (0.13.2)
Requirement already satisfied: numpy>=1.11.2 in d:\tools\anaconda3\lib\site-pack
ages (from scikit-surprise==1.1.0) (1.16.5)
Requirement already satisfied: scipy>=1.0.0 in d:\tools\anaconda3\lib\site-packa
ges (from scikit-surprise==1.1.0) (1.3.1)
Requirement already satisfied: six>=1.10.0 in d:\tools\anaconda3\lib\site-packag
es (from scikit-surprise==1.1.0) (1.12.0)
Building wheels for collected packages: scikit-surprise
  Building wheel for scikit-surprise (setup.py) ... error
  
  building 'surprise.similarities' extension
  error: Microsoft Visual C++ 14.0 is required. Get it with "Microsoft Visual C+
+ Build Tools": https://visualstudio.microsoft.com/downloads/
```
终于看到了VC++RT问题，下载并安装[Microsoft Visual C++ Build Tools](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16)

需要占用500M的磁盘空间



#### refers

[相似度参考](https://surprise.readthedocs.io/en/stable/similarities.html)

