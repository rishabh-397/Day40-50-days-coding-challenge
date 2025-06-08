# Day40-50-days-coding-challenge

# Day 40: Lowest Common Ancestor in BST & Rotate String

## 🧠 Problem 1: Lowest Common Ancestor of a Binary Search Tree

### ✅ Problem Statement:
Given a Binary Search Tree (BST), find the lowest common ancestor (LCA) of two given nodes `p` and `q`.  
The LCA is defined as the lowest node in the tree that has both `p` and `q` as descendants (including the node itself).

### 💡 Constraints:
- Number of nodes in BST: [2, 10^5]
- All node values are unique
- -10^9 <= Node.val <= 10^9
- p != q and both nodes exist in the tree

### 📘 Example 1:
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 8  
Output: 6

### 📘 Example 2:
Input: root = [6,2,8,0,4,7,9,null,null,3,5], p = 2, q = 4  
Output: 2

### ✅ Approach:
- If both p and q are less than the current node, LCA lies in the left subtree.
- If both are greater, LCA lies in the right subtree.
- If one is on the left and one is on the right (or one equals the current node), the current node is the LCA.

---

## 🔄 Problem 2: Rotate String

### ✅ Problem Statement:
Given two strings `s` and `goal`, return `true` if `s` can become `goal` after any number of left shifts.  
A left shift means moving the leftmost character to the end of the string.

### 📘 Example 1:
Input: s = "abcde", goal = "cdeab"  
Output: true

### 📘 Example 2:
Input: s = "abcde", goal = "abced"  
Output: false

### ✅ Approach:
- Concatenate `s + s`
- Check if `goal` is a substring of the concatenated result

### 💡 Constraints:
- 1 <= s.length, goal.length <= 100
- Only lowercase English letters

---

## 📌 Summary:
- The first problem highlights the application of BST properties to find the LCA efficiently.
- The second problem is a clever trick involving string rotation simulation using concatenation.
