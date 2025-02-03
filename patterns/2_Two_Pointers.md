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
my solution is [ezzatziad83 solution](https://leetcode.com/problems/3sum/solutions/6349032/java-solution-by-ezzatziad83-lcqh) take a look at it.
- [11. Container With Most Water](https://leetcode.com/problems/container-with-most-water/)
my solution is [ezzatziad83 solution](https://leetcode.com/problems/container-with-most-water/solutions/6349076/java-solution-by-ezzatziad83-uwcn) take a look at it.

### extra problems:
Majority of two pointers problems are in easy or medium section in LeetCode so, if you understand the basic ideas then it should be solvable without much hints and editorials.

I see 4 bigger categories and many sub categories in it. My recommendation is to start solving these example problems(*), and apply the knowledge to the other problems.

#### 1. Left & Right Pointer (Approaching from both ends of Array)

![Left & Right Pointer](../images/Left%20&%20Right%20Pointer%20(Approaching%20from%20both%20ends%20of%20Array).jpeg)

2 Sum problem
(*) https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/
- my solution is [ezzatziad83 solution](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/solutions/6357646/java-solution-by-ezzatziad83-ydz6) take a look at it.
https://leetcode.com/problems/3sum/
https://leetcode.com/problems/4sum/
https://leetcode.com/problems/number-of-subsequences-that-satisfy-the-given-sum-condition/
https://leetcode.com/problems/two-sum-iv-input-is-a-bst/
https://leetcode.com/problems/sum-of-square-numbers/
https://leetcode.com/problems/boats-to-save-people/
https://leetcode.com/problems/minimize-maximum-pair-sum-in-array/
https://leetcode.com/problems/3sum-with-multiplicity/

Trapping Water
(*) https://leetcode.com/problems/trapping-rain-water/
my solution is [ezzatziad83 solution](https://leetcode.com/problems/trapping-rain-water/solutions/6359151/java-solution-by-ezzatziad83-sm0h) take a look at it.
https://leetcode.com/problems/container-with-most-water/

Next Permutation
(*) https://leetcode.com/problems/next-permutation/
// TODO: add my solution
https://leetcode.com/problems/next-greater-element-iii/
https://leetcode.com/problems/minimum-adjacent-swaps-to-reach-the-kth-smallest-number/

Reversing / Swapping
https://leetcode.com/problems/valid-palindrome/
(*) https://leetcode.com/problems/reverse-string/
my solution is [ezzatziad83 solution](https://leetcode.com/problems/reverse-string/solutions/6363389/java-solution-by-ezzatziad83-1aja) take a look at it.
https://leetcode.com/problems/reverse-vowels-of-a-string/
https://leetcode.com/problems/valid-palindrome-ii/
https://leetcode.com/problems/reverse-only-letters/
https://leetcode.com/problems/remove-element/
https://leetcode.com/problems/sort-colors/
https://leetcode.com/problems/flipping-an-image/
https://leetcode.com/problems/squares-of-a-sorted-array/
https://leetcode.com/problems/sort-array-by-parity/
https://leetcode.com/problems/sort-array-by-parity-ii/
https://leetcode.com/problems/pancake-sorting/
https://leetcode.com/problems/reverse-prefix-of-word/
https://leetcode.com/problems/reverse-string-ii/
https://leetcode.com/problems/reverse-words-in-a-string/
https://leetcode.com/problems/reverse-words-in-a-string-iii/

Others
https://leetcode.com/problems/bag-of-tokens/
https://leetcode.com/problems/di-string-match/
https://leetcode.com/problems/minimum-length-of-string-after-deleting-similar-ends/
https://leetcode.com/problems/sentence-similarity-iii/
https://leetcode.com/problems/find-k-closest-elements/
https://leetcode.com/problems/shortest-distance-to-a-character/

#### 2. Slow & Fast Pointers

![Slow & Fast Pointers](../images/Slow%20&%20Fast%20Pointers.jpeg)

Using two pointers with different speed of movement. Typically they starts from the left end, then the first pointer advances fast and give some feedback to the slow pointer and do some calculation.

Linked List Operations
(*) https://leetcode.com/problems/linked-list-cycle/
my solution is [ezzatziad83 solution](https://leetcode.com/problems/linked-list-cycle/solutions/6367858/java-solution-by-ezzatziad83-msg0) take a look at it.
https://leetcode.com/problems/linked-list-cycle-ii/
https://leetcode.com/problems/remove-nth-node-from-end-of-list/
https://leetcode.com/problems/rotate-list/
https://leetcode.com/problems/reorder-list/
https://leetcode.com/problems/palindrome-linked-list/

Cyclic Detection
(*) https://leetcode.com/problems/find-the-duplicate-number/
my solution is [ezzatziad83 solution](https://leetcode.com/problems/find-the-duplicate-number/solutions/6368263/java-solution-by-ezzatziad83-jdv4) take a look at it.
https://leetcode.com/problems/circular-array-loop/

Sliding Window/Caterpillar Method
(*) https://leetcode.com/problems/number-of-subarrays-with-bounded-maximum/
// TODO: add my solution
https://leetcode.com/problems/find-k-th-smallest-pair-distance/
https://leetcode.com/problems/moving-stones-until-consecutive-ii/
https://leetcode.com/problems/count-pairs-of-nodes/
https://leetcode.com/problems/count-binary-substrings/
https://leetcode.com/problems/k-diff-pairs-in-an-array/

Rotation
(*) https://leetcode.com/problems/rotating-the-box/
// TODO: add my solution
https://leetcode.com/problems/rotate-array/

String
(*) https://leetcode.com/problems/string-compression/
// TODO: add my solution
https://leetcode.com/problems/last-substring-in-lexicographical-order/

Remove Duplicate
(*) https://leetcode.com/problems/remove-duplicates-from-sorted-array/
// TODO: add my solution
https://leetcode.com/problems/remove-duplicates-from-sorted-array-ii/
https://leetcode.com/problems/remove-duplicates-from-sorted-list-ii/
https://leetcode.com/problems/duplicate-zeros/

Others
https://leetcode.com/problems/statistics-from-a-large-sample/
https://leetcode.com/problems/partition-labels/
https://leetcode.com/problems/magical-string/
https://leetcode.com/problems/friends-of-appropriate-ages/
https://leetcode.com/problems/longest-mountain-in-array/
https://leetcode.com/problems/shortest-subarray-to-be-removed-to-make-array-sorted/

#### 3. Merging 2 Arrays | Running from beginning of 2 Arrays
Given 2 arrays or lists, then you have to process them with individual pointers.

![Merging 2 Arrays](../images/Merging%202%20Arrays%20Running%20from%20beginning%20of%202%20Arrays.jpeg)

Sorted arrays
(*) https://leetcode.com/problems/merge-sorted-array/
// TODO: add my solution
https://leetcode.com/problems/heaters/
https://leetcode.com/problems/find-the-distance-value-between-two-arrays/

Intersections/LCA like
(*) https://leetcode.com/problems/intersection-of-two-linked-lists/
// TODO: add my solution
https://leetcode.com/problems/intersection-of-two-arrays/
https://leetcode.com/problems/intersection-of-two-arrays-ii/

SubString
(*) https://leetcode.com/problems/implement-strstr/
// TODO: add my solution
https://leetcode.com/problems/longest-word-in-dictionary-through-deleting/
https://leetcode.com/problems/long-pressed-name/
https://leetcode.com/problems/longest-uncommon-subsequence-ii/
https://leetcode.com/problems/compare-version-numbers/
https://leetcode.com/problems/camelcase-matching/
https://leetcode.com/problems/expressive-words/

Median Finder
(*) https://leetcode.com/problems/find-median-from-data-stream/
// TODO: add my solution

Meet-in-the-middle / Binary Search
(*) https://leetcode.com/problems/partition-array-into-two-arrays-to-minimize-sum-difference/
// TODO: add my solution
https://leetcode.com/problems/closest-subsequence-sum/
https://leetcode.com/problems/ways-to-split-array-into-three-subarrays/
https://leetcode.com/problems/3sum-closest/
https://leetcode.com/problems/valid-triangle-number/

Others
https://leetcode.com/problems/shortest-unsorted-continuous-subarray/
https://leetcode.com/problems/most-profit-assigning-work/
https://leetcode.com/problems/largest-merge-of-two-strings/
https://leetcode.com/problems/swap-adjacent-in-lr-string/

#### 4. Divide & Conquer | Split & Merge of Array

Divide & conquer is similar to Split & Merge but there is one thing added. First, you need to split the given list into 2 separate lists and then do two pointers approach to merge or unify them. There aren’t many problems.

![Divide & Conquer](../images/Divide%20&%20Conquer%20Split%20&%20Merge%20of%20Array.jpeg)

Partition
(*) https://leetcode.com/problems/partition-list/
// TODO: add my solution

Sorting
(*) https://leetcode.com/problems/sort-list/
// TODO: add my solution