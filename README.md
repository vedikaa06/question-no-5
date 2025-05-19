# question-no-5
Solution to the question no 5 on leet code 

5. Longest Palindromic Substring
Given a string s, return the longest palindromic substring in s.

Simple Explanation:
Main idea: A palindrome reads the same forwards and backwards. This code checks each character (and pairs of characters) in the string as a center and expands outward to find the longest palindrome.

How it works:

Loop through each character in the string.

For each character:

Check for odd-length palindromes (centered at that character).

Check for even-length palindromes (centered between that character and the next).

Use a helper method expandFromCenter to expand outwards while characters match.

Keep track of the longest palindrome found.

Helper method (expandFromCenter):

Starts at the given center.

Expands to the left and right as long as the characters match.

Returns the palindromic substring found.

Example:
For input "babad", it checks:

Center at "b" → finds "bab"

Center at "a" → finds "aba"
Returns the longest one: either "bab" or "aba".

This approach efficiently finds the longest palindrome in O(n²) time.
