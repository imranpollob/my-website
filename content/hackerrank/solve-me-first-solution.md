---
title: "Hackerrank - Solve Me First solution"
subtitle: ""
summary: "Hackerrank - Solve Me First solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['warmup', 'algorithms', 'problem-solving', 'hackerrank']
date: 2021-07-02
lastmod: 2021-07-02
featured: false
draft: false
linktitle: "Solve Me First"
type: book
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