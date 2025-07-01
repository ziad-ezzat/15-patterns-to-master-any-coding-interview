# Matrix Traversal
Matrix Traversal involves traversing elements in a matrix using different techniques (DFS, BFS, etc.).

Use this pattern for problems involving traversing 2D grids or matrices horizontally, vertically or diagonally.

## Sample Problem
Perform flood fill on a 2D grid. Change all the cells connected to the starting cell to new color.

Example:

Input: image = [[1,1,1],[1,1,0],[1,0,1]], sr = 1, sc = 1, newColor = 2
Output: [[2,2,2],[2,2,0],[2,0,1]]
Explanation:

Use DFS or BFS to traverse the matrix starting from the given cell.
Change the color of the connected cells to the new color.

## LeetCode Problems
- [.733. Flood Fill (Easy)](https://leetcode.com/problems/flood-fill/)
- [.200. Number of Islands (Medium)](https://leetcode.com/problems/number-of-islands/)
- [.130. Surrounded Regions (Medium)](https://leetcode.com/problems/surrounded-regions/)