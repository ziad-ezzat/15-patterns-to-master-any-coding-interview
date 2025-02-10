# Prefix Sum
Prefix Sum involves preprocessing an array to create a new array where each element at index i represents the sum of the array from the start up to i. This allows for efficient sum queries on subarrays. The prefix sum array can be created in O(n) time and allows for O(1) time sum queries on subarrays.

## sample problem:
Given an array nums, answer multiple queries about the sum of elements within a specific range [i, j].

Example:

Input: nums = [1, 2, 3, 4, 5, 6], i = 1, j = 3
Output: 9

Explanation:

Preprocess the array A to create a prefix sum array: P = [1, 3, 6, 10, 15, 21].
To find the sum between indices i and j, use the formula: P[j] - P[i-1].

Implementation:

```java
class Solution {
    public int sumRange(int i, int j) {
        int[] P = new int[nums.length];
        P[0] = nums[0];
        for (int k = 1; k < nums.length; k++) {
            P[k] = P[k-1] + nums[k];
        }
        return P[j] - (i > 0 ? P[i-1] : 0);
    }
}
```

## LeetCode Problems:
- [303. Range Sum Query - Immutable](https://leetcode.com/problems/range-sum-query-immutable/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/range-sum-query-immutable/solutions/6340163/100-java-solution-by-ezzatziad83-dr2y) take a look at it.
- [525. Contiguous Array](https://leetcode.com/problems/contiguous-array/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/contiguous-array/solutions/6340393/java-solution-by-ezzatziad83-63wa/) take a look at it.
- [560. Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/subarray-sum-equals-k/solutions/6340439/java-solution-by-ezzatziad83-kw66/) take a look at it.
