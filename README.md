LeetCode Solutions:

| # | File Name               | LeetCode Problem         | Difficulty |
| - | ----------------------- | ------------------------ | ---------- |
| 1 | `Solution-01-3524.java` | Find X Value of Array II | Hard       |
| 2 | `Solution-02-47.java`   | Permutations II          | Medium     |
| 3 | `Solution-03-228.java`  | Summary Ranges           | Easy       |
| 4 | `Solution-04-283.java`  | Move Zeroes              | Easy       |
| 5 | `Solution-05-274.java`  | H-Index                  | Medium     |
| 6 | `Solution-06-164.java`  | Maximum Gap              | Medium     |
| 7 | `Solution-07-275.java`  | H-Index II               | Medium     |

1. Find X Value of Array II — LeetCode 3524
Problem Description

Given an array and a series of queries, determine the required X value for each query based on the array values and the given operations.

Approach
Process the array according to the required query operations.
Maintain the necessary state efficiently.
Use appropriate mathematical/array operations to avoid unnecessary repeated computation.
Return the result for every query.
Test Cases

Test Case 1

Input:
nums = [1,2,3,4,5]
queries = [[0,1],[1,2]]

Expected Output:
[1,2]

Test Case 2

Input:
nums = [2,3,4]
queries = [[0,2]]

Expected Output:
[2]

Test Case 3

Input:
nums = [5,5,5]
queries = [[0,0],[1,2]]

Expected Output:
[5,5]
2. Permutations II — LeetCode 47
Problem Description

Given an array that may contain duplicate numbers, return all possible unique permutations.

Approach
Sort the array so duplicate values are adjacent.
Use backtracking to construct permutations.
Track which elements have already been used.
Skip duplicate elements at the same recursion level.
Store every complete permutation.
Test Cases

Test Case 1

Input:
nums = [1,1,2]

Expected Output:
[[1,1,2],
 [1,2,1],
 [2,1,1]]

Test Case 2

Input:
nums = [1,2,3]

Expected Output:
[
 [1,2,3],
 [1,3,2],
 [2,1,3],
 [2,3,1],
 [3,1,2],
 [3,2,1]
]

Test Case 3

Input:
nums = [1,1,1]

Expected Output:
[[1,1,1]]
3. Summary Ranges — LeetCode 228
Problem Description

Given a sorted array of unique integers, summarize consecutive numbers into ranges.

For example, consecutive values such as 4,5,6,7 are represented as 4->7.

Approach
Traverse the array from left to right.
Store the starting value of the current range.
Continue while consecutive numbers are found.
If the range contains one number, add only that number.
Otherwise, add the range using start->end.
Test Cases

Test Case 1

Input:
nums = [0,1,2,4,5,7]

Expected Output:
["0->2","4->5","7"]

Test Case 2

Input:
nums = [0,2,3,4,6,8,9]

Expected Output:
["0","2->4","6","8->9"]

Test Case 3

Input:
nums = []

Expected Output:
[]

Test Case 4

Input:
nums = [5]

Expected Output:
["5"]
4. Move Zeroes — LeetCode 283
Problem Description

Move all zeroes in an integer array to the end while maintaining the relative order of the non-zero elements.

The operation should be performed in-place.

Approach
Maintain a pointer for the position where the next non-zero element should be placed.
Traverse the array.
Move every non-zero value to the correct position.
Fill the remaining positions with zeroes.
Test Cases

Test Case 1

Input:
nums = [0,1,0,3,12]

Expected Output:
[1,3,12,0,0]

Test Case 2

Input:
nums = [0,0,1]

Expected Output:
[1,0,0]

Test Case 3

Input:
nums = [1,2,3]

Expected Output:
[1,2,3]

Test Case 4

Input:
nums = [0,0,0]

Expected Output:
[0,0,0]
5. H-Index — LeetCode 274
Problem Description

Given an array where citations[i] represents the number of citations received by a research paper, calculate the researcher's H-Index.

The H-Index is the maximum value h such that the researcher has at least h papers with at least h citations each.

Approach
Sort the citation array.
Traverse the sorted array.
For each position, calculate how many papers have at least the current number of citations.
Find the maximum valid H-Index.
Test Cases

Test Case 1

Input:
citations = [3,0,6,1,5]

Expected Output:
3

Test Case 2

Input:
citations = [1,3,1]

Expected Output:
1

Test Case 3

Input:
citations = [0,0,0]

Expected Output:
0

Test Case 4

Input:
citations = [10,8,5,4,3]

Expected Output:
4
6. Maximum Gap — LeetCode 164
Problem Description

Given an integer array, find the maximum difference between two successive elements after sorting the array.

The expected solution should use better than O(n log n) time.

Approach
Find the minimum and maximum values.
Use buckets to avoid explicitly sorting the entire array.
Store the minimum and maximum value for each bucket.
Compare the minimum value of the current bucket with the maximum value of the previous non-empty bucket.
Track the largest gap.
Test Cases

Test Case 1

Input:
nums = [3,6,9,1]

Expected Output:
3

Test Case 2

Input:
nums = [10]

Expected Output:
0

Test Case 3

Input:
nums = [1,10000000]

Expected Output:
9999999

Test Case 4

Input:
nums = [1,1,1,1]

Expected Output:
0
7. H-Index II — LeetCode 275
Problem Description

Given a sorted array of citations in ascending order, calculate the H-Index.

Unlike LeetCode 274, the citations are already sorted, allowing a binary-search solution.


Approach
Use binary search.
For index mid, calculate the number of papers having at least citations[mid] citations.
If the number of papers is at least citations[mid], try to find a larger H-Index.
Otherwise, search the other half.
Return the maximum valid H-Index.
Test Cases

Test Case 1

Input:
citations = [0,1,3,5,6]

Expected Output:
3

Test Case 2

Input:
citations = [1,2,100]

Expected Output:
2

Test Case 3

Input:
citations = [0,0,0]

Expected Output:
0

Test Case 4

Input:
citations = [10,10,10]

Expected Output:
3


Learning Objectives:
Practice array traversal and manipulation.
Understand backtracking and duplicate handling.
Learn two-pointer techniques.
Practice sorting-based solutions.
Understand bucket-based algorithms.
Apply binary search to sorted data.
Analyze time and space complexity.
Improve Java problem-solving skills through LeetCode practice.

<!---LeetCode Topics Start-->
# LeetCode Topics
## Array
|  |
| ------- |
| [0073-set-matrix-zeroes](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0073-set-matrix-zeroes) |
| [0079-word-search](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0079-word-search) |
| [0105-construct-binary-tree-from-preorder-and-inorder-traversal](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0105-construct-binary-tree-from-preorder-and-inorder-traversal) |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
| [0212-word-search-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0212-word-search-ii) |
## String
|  |
| ------- |
| [0076-minimum-window-substring](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0076-minimum-window-substring) |
| [0079-word-search](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0079-word-search) |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
| [0212-word-search-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0212-word-search-ii) |
| [0387-first-unique-character-in-a-string](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0387-first-unique-character-in-a-string) |
## Backtracking
|  |
| ------- |
| [0079-word-search](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0079-word-search) |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
| [0212-word-search-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0212-word-search-ii) |
## Depth-First Search
|  |
| ------- |
| [0079-word-search](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0079-word-search) |
## Matrix
|  |
| ------- |
| [0073-set-matrix-zeroes](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0073-set-matrix-zeroes) |
| [0079-word-search](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0079-word-search) |
| [0212-word-search-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0212-word-search-ii) |
## Hash Table
|  |
| ------- |
| [0073-set-matrix-zeroes](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0073-set-matrix-zeroes) |
| [0076-minimum-window-substring](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0076-minimum-window-substring) |
| [0105-construct-binary-tree-from-preorder-and-inorder-traversal](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0105-construct-binary-tree-from-preorder-and-inorder-traversal) |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
| [0387-first-unique-character-in-a-string](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0387-first-unique-character-in-a-string) |
## Dynamic Programming
|  |
| ------- |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
## Trie
|  |
| ------- |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
| [0212-word-search-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0212-word-search-ii) |
## Memoization
|  |
| ------- |
| [0140-word-break-ii](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0140-word-break-ii) |
## Queue
|  |
| ------- |
| [0387-first-unique-character-in-a-string](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0387-first-unique-character-in-a-string) |
## Counting
|  |
| ------- |
| [0387-first-unique-character-in-a-string](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0387-first-unique-character-in-a-string) |
## Sliding Window
|  |
| ------- |
| [0076-minimum-window-substring](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0076-minimum-window-substring) |
## Divide and Conquer
|  |
| ------- |
| [0105-construct-binary-tree-from-preorder-and-inorder-traversal](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0105-construct-binary-tree-from-preorder-and-inorder-traversal) |
## Tree
|  |
| ------- |
| [0105-construct-binary-tree-from-preorder-and-inorder-traversal](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0105-construct-binary-tree-from-preorder-and-inorder-traversal) |
## Binary Tree
|  |
| ------- |
| [0105-construct-binary-tree-from-preorder-and-inorder-traversal](https://github.com/Poojashree2406/Day-10-DSA-practice/tree/master/0105-construct-binary-tree-from-preorder-and-inorder-traversal) |
<!---LeetCode Topics End-->