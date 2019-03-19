# 通过Quandl获取证券交易数据

## 简介

> **[Quandl]**(https://www.quandl.com/) 是一个针对**金融投资行业的大数据平台**，其数据来源包括联合国、世界银行、中央银行等公开数据，核心财务数据来自 CLS集团，Zacks和ICE等，所有的数据源自500多家发布商。![QUANDL](https://www.egouz.com/uploadfile/2017/0919/20170919091540902166.jpg "web页面")

我们可以通过for_free或者share的方式获取到需要的数据样本，获取之后通过下载/编程接口（使用不同的编码）进行数据的调用。

## pthon+quandl

**编程语言：Python 3.7**

需要用到的包是quandl,用于调用接口获取数据。至于大数据存储处理的包就不用多说啦，numpy、pandas是标准开发配置。那么这些python的包从哪里获取呢？最好用的也是较为全面的网站———[官网](https://www.quandl.com/tools/python)或者是[pypi](https://pypi.org/search/?q=quandl)。大数据开发的很多包都可以在**PYPI.ORG**的search网页找到。

.whl文件对应可以使用pip install包管理软件，对于稳定的开发ide来说挺好用。

更快捷的python包导入数据的方式就是下载.tar.gz压缩文件包直接解压缩到python环境路径下的"\Lib\site-packages"即可。

### quanl_data.py
* 导入package
  import numpy as np 
  import pandas as pd
  import quandl, math
