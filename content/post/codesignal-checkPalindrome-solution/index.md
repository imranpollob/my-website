---
title: "Codesignal - checkPalindrome solution"
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
