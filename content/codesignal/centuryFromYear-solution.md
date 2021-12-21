---
title: "Codesignal - centuryFromYear solution"
subtitle: ""
summary: "Codesignal - centuryFromYear solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['codesignal']
date: 2021-07-01
lastmod: 2021-07-01
featured: false
draft: false
linktitle: "centuryFromYear"
type: book
---
Problem [link](https://app.codesignal.com/arcade/intro/level-1/egbueTZRRL5Mm4TXN)

### Solution one:

Basic straight forward solution.

```python
def centuryFromYear(year):
    if year % 100 == 0:
        return year // 100
    return (year // 100) + 1
```

### Solution two:

Interesting solution without using else.

```python
def centuryFromYear(year):
    return (year + 99) // 100
```

### Solution three:

Same theory as above but using `math` library function.

```python
def centuryFromYear(year):
    return math.ceil(year / 100)
}
```

### Solution four:

An different math approach.

```python
def centuryFromYear(year):
    return (year - 1) / 100 + 1;
}
```
