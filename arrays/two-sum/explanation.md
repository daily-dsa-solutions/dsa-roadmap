# Two Sum

## 📝 Problem Statement

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`. You may assume that each input would have exactly one solution, and you may not use the same element twice.

## 🤔 Approach Explained

This solution employs a hash map (dictionary in Python) to efficiently find the pair of numbers that sum up to the target.  Instead of using nested loops which would result in O(n^2) time complexity, it iterates through the input array `nums` only once.  For each number encountered, it calculates the `complement` needed to reach the `target`. It then checks if this `complement` already exists as a key in the `num_map`. If it does, it means we've found the pair, and their indices are returned. If not, the current number and its index are added to the `num_map` for future checks.  This ensures that we only need to traverse the array once to find the solution. The use of a hash map allows for O(1) average-case lookup time.


##  complexity_analysis

- **Time Complexity:** O(n). The algorithm iterates through the input array `nums` once.  Hash map lookups (`complement in num_map`) are on average O(1).

- **Space Complexity:** O(n). In the worst-case scenario, the `num_map` could store all the elements of `nums`, resulting in linear space usage.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
