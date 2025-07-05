# Dynamic Programming 
Dynamic Programming (DP) involves breaking down problems into smaller subproblems and solving them using a bottom-up or top-down approach.

Use this pattern for problems with overlapping subproblems and optimal substructure.

DP itself has multiple sub-patterns. Some of the most important ones are:

Fibonacci Numbers
0/1 Knapsack
Longest Common Subsequence (LCS)
Longest Increasing Subsequence (LIS)
Subset Sum
Matrix Chain Multiplication

### Sample Problem
Calculate the n-th Fibonacci number.

Example:

Input: n = 5
Output: 5 (The first five Fibonacci numbers are 0, 1, 1, 2, 3, 5)
Explanation:

Use a bottom-up approach to calculate the n-th Fibonacci number.
Start with the first two numbers (0 and 1) and iterate to calculate the next numbers like (dp[i] = dp[i - 1] + dp[i - 2]).

## LeetCode Problems
- [.70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)
- [.322. Coin Change](https://leetcode.com/problems/coin-change/)
- [.198. House Robber](https://leetcode.com/problems/house-robber/)
- [.1143. Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/)
- [.416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/)