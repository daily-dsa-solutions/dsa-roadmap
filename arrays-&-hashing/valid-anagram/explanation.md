# Valid Anagram

## 📝 Problem Statement

Given two strings `s` and `t`, return `true` if `t` is an anagram of `s`, and `false` otherwise.

## 🤔 Approach Explained

This solution leverages the fundamental property of anagrams: they contain the same characters with the same frequencies.  The approach elegantly bypasses the need for explicit character counting.  It sorts both input strings alphabetically. If the strings are anagrams, their sorted versions will be identical.  Comparing the sorted strings provides a concise and efficient way to determine if they are anagrams.  The `sorted()` function implicitly handles character frequency comparisons as sorting arranges characters in order, bringing identical characters together for easy comparison.

## complexity_analysis

- **Time Complexity:** O(N log N), where N is the length of the longer string. This is dominated by the sorting operation, which typically has a time complexity of O(N log N) for efficient algorithms like merge sort.

- **Space Complexity:** O(N).  The space used is primarily for storing the sorted versions of the input strings. In the worst case, where all characters are unique, the sorted strings will require space proportional to the length of the original strings.  While Python's `sorted()` function might use extra space internally, it remains proportional to the input size.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
