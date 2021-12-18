---
title: "Leetcode 9 - Palindrome Number solution"
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
Problem [link](https://leetcode.com/problems/palindrome-number)

Solution:

```java
class Solution {
    public boolean isPalindrome(int x) {
        if (x < 0){
            return false;
        }
        
        int rev = 0;
        int real = x;
            
        while (x != 0) {
            rev = rev * 10 + x % 10;
            x = (int) x / 10;
        }
        
        return rev == real;
        
    }
}
```