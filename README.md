# IsPalindrome Algorithm

This repository contains an implementation of the IsPalindrome algorithm in a pseudocode-like format. The algorithm is designed to determine whether a given word is a palindrome or not.

## Algorithm Overview

The `IsPalindrome` algorithm checks whether a given word is a palindrome. A palindrome is a word, phrase, or sequence of characters that reads the same forwards as it does backward.

1. Initialize a boolean variable `isPalindrome` as `true`.
2. Iterate through the characters of the word using a loop, comparing characters from both ends towards the middle.
3. If a character mismatch is found, set `isPalindrome` to `false` and exit the loop.
4. Return the value of the `isPalindrome` variable, indicating whether the word is a palindrome.

## Usage

1. Provide the word string to be tested for palindrome.
2. Run the IsPalindrome algorithm.
3. The algorithm will return true if the provided word is a palindrome, and false otherwise.

## Example
// Example input
word = "level"

// Run the algorithm
result = IsPalindrome(word)

// The result is true, as "level" is a palindrome.

## Pseudocode

```plaintext
ALGORITHM IsPalindrome
VAR
    word: a string representing the word to be tested
    n: the number of characters in the word
    isPalindrome: a boolean variable indicating if the word is a palindrome
BEGIN
    isPalindrome <- true
    FOR i <- 0 TO n/2
        IF word[i] != word[n - i - 1] THEN
            isPalindrome <- false
            BREAK
        END IF
    END FOR
    RETURN isPalindrome
END
