# Monotonic Stack
The Monotonic Stack pattern uses a stack to maintain a sequence of elements in a specific order (increasing or decreasing).

Use this pattern for problems that require finding the next greater or smaller element.

## Sample Problem
Find the next greater element for each element in an array. Output -1 if the greater element doesn’t exist.

Example:

Input: nums = [2, 1, 2, 4, 3]
Output: [4, 2, 4, -1, -1]
Explanation:

Use a stack to keep track of elements for which we haven’t found the next greater element yet.
Iterate through the array, and for each element, pop elements from the stack until you find a greater element.
If the stack is not empty, set the result for index at the top of the stack to current element.
Push the current element onto the stack.

## LeetCode Problems
- [496. Next Greater Element I (Easy)](https://leetcode.com/problems/next-greater-element-i/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/next-greater-element-i/solutions/6514713/java-solution-by-ezzatziad83-dafx) take a look at it.
- [739. Daily Temperatures (Medium)](https://leetcode.com/problems/daily-temperatures/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/daily-temperatures/solutions/6514795/java-solution-by-ezzatziad83-5mp0) take a look at it.
- [84. Largest Rectangle in Histogram (Hard)](https://leetcode.com/problems/largest-rectangle-in-histogram/)