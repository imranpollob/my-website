---
title: "Leetcode 9 - Palindrome Number solution"
subtitle: ""
summary: "Leetcode 9 - Palindrome Number solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21
lastmod: 2021-10-21
featured: false
draft: false
linktitle: "9 - Palindrome Number"
type: book
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