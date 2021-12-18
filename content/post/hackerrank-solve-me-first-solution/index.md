---
title: "Hackerrank - Solve Me First solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['warmup', 'algorithms', 'problem-solving', 'hackerrank']
date: 2021-07-02T15:17:25+06:00
lastmod: 2021-07-02T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/solve-me-first/problem)

### Solution one

Just return the addition of the two numbers.

```python
def solveMeFirst(a,b):
	return a + b
```

### Solution two

Find the addition using library function `sum`. The advantage of the `sum` function is that it can take variable number of arguments. For example, `sum(1, 2, 3, 4)` will also work.

```python
def solveMeFirst(a,b):
	return sum(a, b)
```