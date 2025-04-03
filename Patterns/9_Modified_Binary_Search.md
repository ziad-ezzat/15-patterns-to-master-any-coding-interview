# Modified Binary Search
Modified Binary Search pattern adapts binary search to solve a wider range of problems, such as finding elements in rotated sorted arrays.

Use this pattern for problems involving sorted or rotated arrays where you need to find a specific element.

## Sample Problem
Find an element in a rotated sorted array.

Example:

Input: nums = [4, 5, 6, 7, 0, 1, 2], target = 0
Output: 4
Explanation:

Perform binary search with an additional check to determine which half of the array is sorted.
We then check if the target is within the range of the sorted half.
If it is, we search that half; otherwise, we search the other half.

## LeetCode Problems
- [33. Search in Rotated Sorted Array (Medium)](https://leetcode.com/problems/search-in-rotated-sorted-array/)
- [153. Find Minimum in Rotated Sorted Array (Medium)](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/)
- [240. Search a 2D Matrix II (Medium)](https://leetcode.com/problems/search-a-2d-matrix-ii/)