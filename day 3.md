53. Maximum Subarray
Given an integer array nums, find the subarray with the largest sum, and return its sum.

---------------------------------------
```
class Solution(object):
    def maxSubArray(self, nums):
        res = nums[0]
        total = 0

        for n in nums:
            if total < 0:
                total = 0

            total += n
            res = max(res, total)
        
        return res
```
        
