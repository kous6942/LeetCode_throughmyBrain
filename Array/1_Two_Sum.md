# 1. Two Sum

### Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target. You may assume that each input would have exactly one solution, and you may not use the same element twice. You can return the answer in any order.

 
Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

Example 2:
Input: nums = [3,2,4], target = 6
Output: [1,2]

Example 3:
Input: nums = [3,3], target = 6
Output: [0,1]
 
Constraints:

2 <= nums.length <= 104
-109 <= nums[i] <= 109
-109 <= target <= 109
Only one valid answer exists.
 

# Approach and Understanding
Brute force is my way to go. First I run initialize i and then initialize j positioned as i+1. Here onwards, I run 2 for loops iterating and checking i+j combos through the array.
I place and if condition to check if at any point nums[i] + nums[j] == targer, whenever true; I reach my answer.
Thus, returning the 2 indices: [i,j]
