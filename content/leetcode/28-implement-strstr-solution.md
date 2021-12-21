---
title: "Leetcode 28 - Implement strStr() solution"
subtitle: ""
summary: "Leetcode 28 - Implement strStr() solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21
lastmod: 2021-10-21
featured: false
draft: false
linktitle: "28 - Implement strStr()"
type: book
---
Problem [link](https://leetcode.com/problems/implement-strstr)

Solution:

```java
class Solution {
    public int strStr(String haystack, String needle) {
        int nl = needle.length();

        for(int i = 0; i <= haystack.length() - nl; i = i+1) {
            if (haystack.substring(i, i + nl).equals(needle)) {
                return i;
            }
        }
        
        return -1;
    }
}
```