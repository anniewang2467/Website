---
title: 'Teamwork: R and Python Working Together!'
author: Anyi Wang
date: '2020-05-15'
slug: teamwork-r-and-python-working-together
categories: []
tags: []
description: ''
---
Hello World! 

I'm so excited because... this is my first blogpost EVER!!!

![](/blog/2020-05-15-teamwork-r-and-python-working-together_files/excited.jpg)

Anyways, through Computational Biology and Bioinformatics in my last semester senior year, I have learned a small amount of Python and (a smidge more) and R Studio. Here are some of the basics in each program!


```r
#R code
hi <- "hello"
hi
```

```
## [1] "hello"
```

```r
1+2
```

```
## [1] 3
```

```r
#plot
plot(cars)
```

<img src="/blog/2020-05-15-teamwork-r-and-python-working-together_files/figure-html/cars-1.png" width="672" />



```python
#python code
print(2+2)
```

```
## 4
```



Everybody stand back. I know regular expressions!


```python

import re

string1="We have to extract these numbers 12, 47, 48 The integers numbers are also interesting: 189 2036 314\',\' is a separator, so please extract these numbers 125,789,1450 and also these 564,90456 We like to offer you 7890$ per month in order to complete this task... we are joking"

print(string1)
```

```
## We have to extract these numbers 12, 47, 48 The integers numbers are also interesting: 189 2036 314',' is a separator, so please extract these numbers 125,789,1450 and also these 564,90456 We like to offer you 7890$ per month in order to complete this task... we are joking
```

```python
re.findall(r"\d+",string1)
```

```
## ['12', '47', '48', '189', '2036', '314', '125', '789', '1450', '564', '90456', '7890']
```

And now... what you've all been waiting for! Watch R and Python work togther through the reticulate library!


```r
hi <- "hello"
library(reticulate)
```

```
## Warning: package 'reticulate' was built under R version 3.6.3
```


```python
hi = "world"
print(r.hi,hi)
```

```
## hello world
```


Alright yall: ![](/blog/2020-05-15-teamwork-r-and-python-working-together_files/0A960A51-9A23-4D7E-8AA9-E3976D12159A.jpg)
