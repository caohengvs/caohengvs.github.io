---
title: String类实用
layout: post
categories: c++
tags: std::string
excerpt: String类实用

---

# String类实用

# 需要用到的头文件以及命名空间

```c++
#include<iostream>
using namespace std;
```

# 常用string函数

## int find(string strFind)

+ 注解
  
  查找字符串的位置，并返回首字符的索引，未找到返回-1；

+ 用例
  
  ```c++
  ...
  string strFind = "adbs<end>";
  string strTarget = "<end>";
  int nIndex = strFind.find(strTarget);
  ...
  ```

+ 反向
  
  即反向搜索待查找字符串
  
  ```c++
  int rfind(string strFind);
  ```

## string replace(int nStart, int nCount, string strReplace)

+ 注解
  
  用strReplace,替代从nStart开始包含nStart索引的nCount个字符

+ 用例
  
  ```c++
  ...
  string strReplace= "adbs<end>";
  string strTarget = "<end>";
  string nIndex = strReplace.replace(0,1,strTarget);
  ...
  ```

# 

## regex的运用

```c++
#include<regex>
#include<iostream>
using namespace std;
string strTest = "goal.h";
string strReg = ".h";
string strMatchRst;
// 正则搜索
regex_search(strTest, strReg);
// 正则匹配
regex_match(strTest, strMatch, strReg);
```
