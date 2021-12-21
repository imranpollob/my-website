---
title: "Codesignal - checkPalindrome solution"
subtitle: ""
summary: "Codesignal - checkPalindrome solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['codesignal']
date: 2021-07-01
lastmod: 2021-07-01
featured: false
draft: false
linktitle: "checkPalindrome"
type: book
---
Problem [link](https://app.codesignal.com/arcade/intro/level-1/s5PbmwxfECC52PWyQ)

### Solution one:

Looping through the array from last to first.

```python
def checkPalindrome(inputString):
    r = ""

    for i in range(len(inputString)-1, -1, -1):
        r += inputString[i]

    return inputString == r
```

### Solution two:

Using Python's default syntax.

```python
def checkPalindrome(inputString):
    return inputString == inputString[::-1]
```

### Solution three:

A JavaScript solution.

```js
function checkPalindrome(inputString) {
  return inputString == inputString.split('').reverse().join('')
}
```

### Solution four:

An optimal solution because it's just looping through half of the array.

```python
def checkPalindrome(inputString):
    for i in range(len(inputString) // 2):
        if inputString[i] != inputString[-i - 1]:
            return False
    return True
```
