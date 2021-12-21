---
title: "Leetcode 7 - Reverse Integer solution"
subtitle: ""
summary: "Leetcode 7 - Reverse Integer solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21
lastmod: 2021-10-21
featured: false
draft: false
linktitle: "7 - Reverse Integer"
type: book
---
Problem [link](https://leetcode.com/problems/reverse-integer/)

Solution:

```java
class Solution {
    public int reverse(int x) {
        int rev = 0;
        
        while(x != 0){
            if(rev > Integer.MAX_VALUE / 10 || rev < Integer.MIN_VALUE / 10)
                return 0;
            rev = rev * 10 + x % 10;
            x = x / 10;
        }
        
        return rev;
    }
}
```