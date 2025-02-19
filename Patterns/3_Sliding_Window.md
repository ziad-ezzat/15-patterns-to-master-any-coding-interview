# Sliding Window
Sliding Window pattern is used to find a sub-array or sub-string that satisfies a specific condition, optimizing the time complexity by maintaining a window of elements.

Use this pattern when dealing with problems involving contiguous sub-arrays or sub-strings.

## Sample Problem:
Find the maximum sum of a subarray of size k.

Example:

Input: [2, 1, 5, 1, 3, 2], k=3
Output: 9

Explanation:

Start with the sum of the first k elements.
Slide the window one element at a time, subtracting the element that goes out of the window and adding the new element.
Keep track of the maximum sum encountered.

## LeetCode Problems:

- [643. Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/maximum-average-subarray-i/solutions/6441803/java-solution-by-ezzatziad83-2ep2) take a look at it.
- [3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/longest-substring-without-repeating-characters/solutions/6441845/java-solution-by-ezzatziad83-fd9b) take a look at it.
- [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/minimum-window-substring/solutions/6441961/java-solution-by-ezzatziad83-bzr3) take a look at it.