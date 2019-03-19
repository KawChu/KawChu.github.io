# **Obtaining Stock Exchange Data through Quandl**


## summary

> [**Quandl**] (https://www.quandl.com/) is a large data platform for **financial investment industry**. It's data sources include open data such as the United Nations, the World Bank and the Central Bank. The core financial data are from CLS Group, Zacks and ICE, all of which are from more than 500 publishers.![QUANDL](https://www.egouz.com/uploadfile/2017/0919/20170919091540902166.jpg)

We can get the required data samples by for_free or share, and then call the data by downloading/programming interface (using different encoding).

## pthon+quandl

**Programing language: Python 3.7**

The package you need is quandl, which is used to call the interface to get data. As for big data storage processing packages, it is not necessary to mention that numpy and pandas are standard development configurations. So where do these Python packages come from? The best website to use is also a more comprehensive website - [official website](https://www.quandl.com/tools/python) or [pypi](https://pypi.org/search/?q=quandl). Many packages for big data development can be found on the search page of **PYPI.ORG**.

.whl files can be managed using PIP install package management software, which is very useful for the stable development of ides.

A faster way for Python packages to import data is to download .tar.gz compressed file packages and decompress them directly into "\Lib\site-packages" under the python environment path.

### quanl_data.py
```
  import numpy as np 
  import pandas as pd
  import quandl, math
  //import the required packet
  
  quandl_code = "NASDAQOMX/NQCN9000CNY"
  //setting the Coding of Securities Data Samples
  
  df = quandl.get(quandl_code)
  //get data by calling the interface and store it in the dataframe
  
  df.fillna(value=0)
  //fill nan_null with 0
```

