# Two Sum

## 📝 Problem Statement

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

## 🤔 Approach Explained

This solution leverages a hash map (dictionary in Python) to efficiently find the pair of numbers that sum up to the target.  The algorithm iterates through the input array `nums` only once. For each number encountered, it calculates the `complement` needed to reach the `target`. It then checks if this `complement` already exists as a key in the `num_map`. If it does, it means we've found the pair, and their indices are returned.  If the complement is not found, the current number and its index are added to the `num_map` for future comparisons. If no such pair is found after iterating through the entire array, an empty list is returned.  This single-pass approach significantly improves efficiency compared to brute-force methods.

##  complexity_analysis

*   **Time Complexity:** O(n) - The algorithm iterates through the input array `nums` once.  Hash map lookups (`complement in num_map`) take O(1) on average.

*   **Space Complexity:** O(n) - In the worst-case scenario, the `num_map` could store all the numbers from the input array, resulting in a space complexity proportional to the size of the input.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
