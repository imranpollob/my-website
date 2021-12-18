---
title: "Codesignal - shapeArea solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['codesignal']
date: 2021-07-01T15:17:25+06:00
lastmod: 2021-07-01T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://app.codesignal.com/arcade/intro/level-2/yuGuHvcCaFCKk56rJ)

The solutions here are quite similar in a sense that all are based on math.

### Solution one:

```python
def shapeArea(n):
    return n*n + (n-1)*(n-1)
```

### Solution two:

```python
def shapeArea(n):
    return n**2 + (n-1)**2
```

### Solution three:

```python
def shapeArea(n):
    return 2*n*(n-1) + 1
```

### Solution four:

```python
def shapeArea(n):
    result = 1

    for i in range(n):
        result += 4 * i

    return result
```
