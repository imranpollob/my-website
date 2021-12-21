---
title: "Leetcode 1480 - Running Sum of 1d Array solution"
subtitle: ""
summary: "Leetcode 1480 - Running Sum of 1d Array solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['leetcode']
date: 2021-10-21
lastmod: 2021-10-21
featured: false
draft: false
linktitle: "1480 - Running Sum of 1d Array"
type: book
---
Problem [link](https://leetcode.com/problems/running-sum-of-1d-array)

To solve this problem we are storing the summation in place.

```python
class Solution:
    def runningSum(self, nums: List[int]) -> List[int]:
        for i in range(1, len(nums)):
            nums[i] = nums[i] + nums[i-1]
            
        return nums
```

```java
class Solution {
   public int[] runningSum(int[] nums) {
       for(int i = 1; i < nums.length; i++){
           nums[i] = nums[i] + nums[i-1];
       }
       return nums;
   }
}
```

**Time complexity: O(n)
Space complexity: O(n)**