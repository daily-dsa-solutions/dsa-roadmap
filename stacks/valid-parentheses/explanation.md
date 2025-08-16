# Valid Parentheses

## 📝 Problem Statement

Given a string s containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid.

## 🤔 Approach Explained

This solution employs a stack-based approach to efficiently determine the validity of parenthesis pairings in a given string.  The algorithm iterates through the input string character by character. If a closing parenthesis (')', '}', or ']') is encountered, it checks the top element of the stack. The stack stores the opening parentheses encountered so far.  A hash map (`mapping`) provides a quick lookup to determine the corresponding opening parenthesis for each closing parenthesis.  If a match is found (the top of the stack is the corresponding opening parenthesis), the pair is considered valid and the opening parenthesis is popped from the stack. If no match is found or the stack is empty, the string is invalid, and the function returns `False`. If the character is an opening parenthesis, it is simply pushed onto the stack. Finally, if the stack is empty after processing the entire string, it means all opening parentheses have been correctly matched with closing parentheses, and the function returns `True`; otherwise, it returns `False`. The use of '#' as a default value when the stack is empty during a pop operation ensures robustness against potential exceptions.

##  complexity_analysis

-   **Time Complexity:** O(n), where n is the length of the input string. The algorithm iterates through the string once.  Stack operations (push and pop) take constant time on average.

-   **Space Complexity:** O(n) in the worst case. The space used by the stack is proportional to the maximum nesting depth of parentheses in the input string. In the worst-case scenario (e.g., a string with all opening parentheses), the stack size will be equal to the length of the string.


---

📺 [Link to YouTube Video Explanation](your-youtube-link-here)
