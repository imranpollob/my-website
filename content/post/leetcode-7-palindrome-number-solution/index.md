---
title: "Leetcode 9 - Palindrome Number solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21T15:17:25+06:00
lastmod: 2021-10-21T15:17:25+06:00
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