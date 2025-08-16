# Two Sum

## 📝 Problem Statement

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`. You may assume that each input would have exactly one solution, and you may not use the same element twice.

## 🤔 Approach Explained

This solution employs a hash map (dictionary in Python) to efficiently find the two numbers that sum up to the target.  The algorithm iterates through the input array `nums` only once. For each number encountered, it calculates the `complement` needed to reach the `target`. It then checks if this `complement` already exists as a key in the `num_map`. If it does, it means the pair has been found, and the indices are returned.  If the complement is not found, the current number and its index are added to the `num_map` for future comparisons.  This avoids nested loops, resulting in a significant performance improvement compared to brute-force approaches. The use of a hash map allows for O(1) average-case lookup time.


## complexity_analysis

- **Time Complexity:** O(n) - The algorithm iterates through the input array once.  Hash map lookups (on average) take constant time.

- **Space Complexity:** O(n) - In the worst-case scenario, the `num_map` could store all the numbers from the input array.  The space used is proportional to the size of the input.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
