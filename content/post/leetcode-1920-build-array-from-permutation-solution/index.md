---
title: "Leetcode 1920 - Build Array from Permutation solution"
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