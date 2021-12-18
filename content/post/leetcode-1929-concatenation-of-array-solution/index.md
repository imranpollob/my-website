---
title: "Leetcode 1929 - Concatenation of Array solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-22
lastmod: 2021-10-22
featured: false
draft: false
---
Problem [link](https://leetcode.com/problems/concatenation-of-array)

Solution One:

```python
class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        return nums * 2
```

Solution Two:

```java
class Solution {
    public int[] getConcatenation(int[] nums) {
        int len = nums.length;
        int[] nums2 = new int[len*2];
        
        for(int i = 0; i < len; i++) {
            nums2[i] = nums[i];
            nums2[i + len] = nums[i];
        }
        
        return nums2;
    }
}
```