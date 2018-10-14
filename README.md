# leetcode1
"""
Given an array of integers, return indices of the two numbers such that they add up to a specific target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
Example:
Given nums = [2, 7, 11, 15], target = 9,
Because nums[0] + nums[1] = 2 + 7 = 9,
return [0, 1].
"""
print(kick it!)

def TwoSum(nums, target):
    dic = dict()
    for index, value in enumerate(nums):
        #[(0,2), (1,7), (2,11), (3,15)], (index,value)
        sub = target - value
        if sub in dic:
            return [dic[sub], index]
        else:
            dic[value] = index
            
nums = [2, 7, 11, 15]
target = 9
result = TwoSum(nums, target)
result
