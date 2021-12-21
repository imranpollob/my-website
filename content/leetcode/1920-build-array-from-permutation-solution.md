---
title: "Leetcode 1920 - Build Array from Permutation solution"
subtitle: ""
summary: "Leetcode 1920 - Build Array from Permutation solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-22
lastmod: 2021-10-22
featured: false
draft: false
linktitle: "1920 - Build Array from Permutation"
type: book
---
Problem [link](https://leetcode.com/problems/build-array-from-permutation)

Solution One:

```java
class Solution {
    public int[] buildArray(int[] nums) {
        int[] ans = new int[nums.length];
        
        for(int i = 0; i < nums.length; i++){
            ans[i] = nums[nums[i]];
        }
        
        return ans;
    }
}
```

```python
class Solution:
    def buildArray(self, nums: List[int]) -> List[int]:
        ans = []
        
        for i in range(len(nums)):
            ans.append(nums[nums[i]])
            
        return ans
```