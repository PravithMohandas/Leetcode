# Integer to Roman

- **Problem:** 12
- **Difficulty:** Medium
- **URL:** https://leetcode.com/problems/integer-to-roman/
- **Language:** Python3
- **Accepted at:** 2026-09-09 14:32 (LeetCode display time; seconds not shown)
- **Submission ID:** 2136124560
- **Status:** Accepted

## Summary

Convert an integer from 1 through 3999 to its Roman numeral representation, including the standard subtractive pairs such as IV, IX, XL, XC, CD, and CM.

## Approach

Walk the Roman symbol/value pairs from largest to smallest. Append each symbol while its value fits in the remaining number, subtracting it each time. Including the subtractive pairs in descending order handles those cases with the same greedy loop.

## Complexity

- **Time:** O(1), since the input is bounded by 3999 and the symbol table has a fixed size.
- **Auxiliary space:** O(1), excluding the returned string; its maximum length is bounded by the input range.
