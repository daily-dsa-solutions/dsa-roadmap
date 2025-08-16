# Longest Consecutive Sequence

## 📝 Problem Statement

Given an unsorted array of integers `nums`, find the length of the longest consecutive elements sequence.

## 🤔 Approach Explained

This solution leverages a set data structure to efficiently find the longest consecutive sequence of numbers.  The core idea is to iterate through the unique numbers (using a set eliminates duplicates). For each number, it checks if it's the start of a consecutive sequence (by verifying that the preceding number is not present in the set). If it is the start, it then iteratively extends the sequence until it encounters a gap (a number not present in the set).  The length of the longest sequence found during this process is then returned.  Using a set provides O(1) lookup time, making the overall algorithm very efficient.

## complexity_analysis

*   **Time Complexity:** O(n), where n is the length of the input array `nums`.  Although there are nested loops, each number is only visited and processed once (or at most twice, depending on how sequences overlap).  The set lookup (`in num_set`) is O(1) on average.

*   **Space Complexity:** O(n) in the worst case. This is because the set `num_set` could potentially store all unique numbers from the input array.  In the best case (all numbers are unique and form a single sequence), space complexity would also be O(n).


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
