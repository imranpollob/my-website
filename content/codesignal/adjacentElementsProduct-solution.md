---
title: "Codesignal - adjacentElementsProduct solution"
subtitle: ""
summary: "Codesignal - adjacentElementsProduct solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['codesignal']
date: 2021-07-01
lastmod: 2021-07-01
featured: false
draft: false
linktitle: "adjacentElementsProduct"
type: book
---
Problem [link](https://app.codesignal.com/arcade/intro/level-2/xzKiBHjhoinnpdh6m)

### Solution one:

We are gonna find the ajacent product and store the maximum value to `best` variable.

```python
def adjacentElementsProduct(inputArray):
    best = inputArray[0] * inputArray[1]

    for i in range(1, len(inputArray) - 1):
        temp = inputArray[i] * inputArray[i + 1]

        if temp > best:
            best = temp

    return best
```

### Solution two:

This solution is same as above but fancier.

```python
def adjacentElementsProduct(inputArray):
    return max([inputArray[i] * inputArray[i+1] for i in range(len(inputArray)-1)])
```

### Solution three:

This is a different approach but it's not optimal because we have to maintain an array for this.

```js
def adjacentElementsProduct(inputArray):
    products = []

    for i in range(len(inputArray)-1):
        products.append(inputArray[i]*inputArray[i+1])

    return max(products)
```
