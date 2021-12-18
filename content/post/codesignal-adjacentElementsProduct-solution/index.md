---
title: "Codesignal - adjacentElementsProduct solution"
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
