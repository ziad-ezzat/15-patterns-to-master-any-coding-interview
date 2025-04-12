# Binary Tree Traversal
Binary Tree Traversal involves visiting all the nodes in a binary tree in a specific order.

PreOrder: root -> left -> right
InOrder: left -> root -> right
PostOrder: left -> right -> root

## Sample Problem:
Problem Statement: Perform inorder traversal of a binary tree.

Example:

Input: root = [1, null, 2, 3]
Output: [1, 3, 2]
Explanation:

Inorder traversal visits nodes in the order: left, root, right.
Use recursion or a stack to traverse the tree in this order.

## LeetCode Problems:
- [294. Binary Tree Inorder Traversal (Easy)](https://leetcode.com/problems/binary-tree-inorder-traversal/)
class Solution {
    public List<Integer> inorderTraversal(TreeNode root) {
        List<Integer> result = new ArrayList<>();
        inorderHelper(root, result);
        return result;
    }

    private void inorderHelper(TreeNode node, List<Integer> result) {
        if (node == null) return;
        inorderHelper(node.left, result);
        result.add(node.val);
        inorderHelper(node.right, result);
    }
}
- [230. Kth Smallest Element in a BST (Medium)](https://leetcode.com/problems/kth-smallest-element-in-a-bst/)
class Solution {
    public int kthSmallest(TreeNode root, int k) {
        List<Integer> result = new ArrayList<>();
        inorderHelper(root, result);
        return result.get(k - 1);
    }

    private void inorderHelper(TreeNode node, List<Integer> result) {
        if (node == null) return;
        inorderHelper(node.left, result);
        result.add(node.val);
        inorderHelper(node.right, result);
    }
}
- [124. Binary Tree Maximum Path Sum (Hard)](https://leetcode.com/problems/binary-tree-maximum-path-sum/)
class Solution {
    public int maxPathSum(TreeNode root) {
        int[] maxSum = {Integer.MIN_VALUE};
        maxPathHelper(root, maxSum);
        return maxSum[0];
    }

    private int maxPathHelper(TreeNode node, int[] maxSum) {
        if (node == null) return 0;
        int left = Math.max(0, maxPathHelper(node.left, maxSum));
        int right = Math.max(0, maxPathHelper(node.right, maxSum));
        maxSum[0] = Math.max(maxSum[0], left + right + node.val);
        return Math.max(left, right) + node.val;
    }
}