---
title: "Leetcode 283 - Move Zeros solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-08T15:17:25+06:00
lastmod: 2021-10-08T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://leetcode.com/problems/move-zeroes/)

### Solution one:

To solve this problem we will use two points. One pointer will track zero another will track nonzero numbers. Zero pointer will be increamented if it finds zero in the list otherwise the numbers on Zero and Nonzero pointers swap their values and both pointers will be increamented.

```python
class Solution:
    def moveZeroes(self, nums: List[int]) -> None:
        """
        Do not return anything, modify nums in-place instead.
        """
        zero = 0
        nonzero = 0
        
        while zero < len(nums):
            if nums[zero] == 0:
                zero += 1
            else:
                nums[zero], nums[nonzero] = nums[nonzero], nums[zero]
                zero += 1
                nonzero += 1
        
        return nums
```