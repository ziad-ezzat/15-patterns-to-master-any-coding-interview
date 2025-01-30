# Two Pointers
The Two Pointers pattern involves using two pointers to iterate through an array or list, often used to find pairs or elements that meet specific criteria.

Use this pattern when dealing with sorted arrays or lists where you need to find pairs that satisfy a specific condition.

## sample problem:
Find two numbers in a sorted array that add up to a target value.

Example:

Input: nums = [1, 2, 3, 4, 6], target = 6
Output: [1, 3]

Explanation:

Initialize two pointers, one at the start (left) and one at the end (right) of the array.
Check the sum of the elements at the two pointers.
If the sum equals the target, return the indices.
If the sum is less than the target, move the left pointer to the right.
If the sum is greater than the target, move the right pointer to the left.

Implementation:

```java
class Solution {
    public int[] twoSum(int[] nums, int target) {
        int left = 0, right = nums.length - 1;
        while (left < right) {
            int sum = nums[left] + nums[right];
            if (sum == target) {
                return new int[] {left, right};
            } else if (sum < target) {
                left++;
            } else {
                right--;
            }
        }
        return new int[] {-1, -1};
    }
}
```

## LeetCode Problems:
- [167. Two Sum II - Input array is sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/solutions/6348846/java-solution-by-ezzatziad83-qmzi) take a look at it.
- [15. 3Sum](https://leetcode.com/problems/3sum/)
- [11. Container With Most Water](https://leetcode.com/problems/container-with-most-water/)

### to be continued...