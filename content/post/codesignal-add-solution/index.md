---
title: "Codesignal - add solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['codesignal']
date: 2021-03-11T15:29:58+06:00
lastmod: 2021-03-11T15:29:58+06:00
featured: false
draft: false
---
Problem [link](https://app.codesignal.com/arcade/intro/level-1/jwr339Kq6e3LQTsfa)

### Solution one:

Simply return the summation of the two numbers.

```python
def add(param1, param2):
    return param1 + param2
```

### Solution two:

Find the addition using library function `sum`. The advantage of the `sum` function is that it can take variable number of arguments. For example, `sum(1, 2, 3, 4)` will also work.

```python
def add(param1, param2):
    return sum(param1, param2)
```