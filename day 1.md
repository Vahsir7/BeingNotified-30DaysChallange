<h1> Question Day1</h1>
<b>
Given an array nums of size n, return the majority element.<br>
The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.  
</b>

<hr>

```
  class Solution:
    def majorityElement(self, nums: List[int]) -> int:
        l=len(nums)
        if l==1:
            return nums[0]
        nums=sorted(nums)
        if(nums[:l//2][0] in nums[l//2:]):
            return nums[:l//2][0]
        else:
            return nums[l//2:][0]
```
