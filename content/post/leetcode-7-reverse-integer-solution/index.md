---
title: "Leetcode 7 - Reverse Integer solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21
lastmod: 2021-10-21
featured: false
draft: false
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