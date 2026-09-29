# Valid Palindrome

LeetCode solution for the **Valid Palindrome** problem.

## Problem

Given a string `s`, determine whether it is a palindrome after:

- considering only letters and digits
- ignoring uppercase/lowercase differences

## Approach

The solution uses the **two-pointer technique**.

Two pointers start at opposite ends of the string:

- `left` moves from left to right
- `right` moves from right to left
- non-alphanumeric characters are skipped
- valid characters are compared case-insensitively

If any pair does not match, the function returns `False`.

If all mirror pairs match, it returns `True`.

## Complexity

- Time: **O(n)**
- Space: **O(1)**

## Examples

```text
"A man, a plan, a canal: Panama" → True
"race a car" → False
" " → True
"0P" → False
