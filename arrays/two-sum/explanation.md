# Two Sum

## 📝 Problem Statement

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`. You may assume that each input would have exactly one solution, and you may not use the same element twice.

## 🤔 Approach Explained

This solution leverages a hash map (dictionary in Python) to efficiently find the two numbers that sum up to the target.  It iterates through the input array `nums` only once. For each number encountered, it calculates the `complement` needed to reach the `target`.  It then checks if this `complement` already exists as a key in the `num_map`. If it does, it means the pair has been found, and the indices are returned. If not, the current number and its index are added to the `num_map`.  This allows for quick lookups in subsequent iterations. The use of a hash map avoids the need for nested loops, resulting in a significant performance improvement compared to brute-force approaches.  If no solution is found after iterating through the entire array, an empty list is returned.


##  complexity_analysis

- **Time Complexity:** O(n). The algorithm iterates through the input array `nums` once.  Hash map lookups (`complement in num_map`) take constant time on average (O(1)).

- **Space Complexity:** O(n). In the worst-case scenario, the `num_map` hash map could store all the elements of the input array `nums`.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
