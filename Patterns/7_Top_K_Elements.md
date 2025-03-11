# Top ‘K’ Elements
The Top ‘K’ Elements pattern finds the top k largest or smallest elements in an array or stream of data using heaps or sorting.

## Sample Problem
Find the k-th largest element in an unsorted array.

Example:

Input: nums = [3, 2, 1, 5, 6, 4], k = 2
Output: 5
Explanation:

Use a min-heap of size k to keep track of the k largest elements.
Iterate through the array, adding elements to the heap.
If the heap size exceeds k, remove the smallest element from the heap.
The root of the heap will be the k-th largest element.

## LeetCode Problems
- [215. Kth Largest Element in an Array (Medium)](https://leetcode.com/problems/kth-largest-element-in-an-array/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/kth-largest-element-in-an-array/solutions/6523619/java-solution-by-ezzatziad83-5wsb) take a look at it.
- [347. Top K Frequent Elements (Medium)](https://leetcode.com/problems/top-k-frequent-elements/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/top-k-frequent-elements/solutions/6523639/java-solution-by-ezzatziad83-qwyr) take a look at it.
- [373. Find K Pairs with Smallest Sums (Medium)](https://leetcode.com/problems/find-k-pairs-with-smallest-sums/)