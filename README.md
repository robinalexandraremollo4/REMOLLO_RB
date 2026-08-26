# ECE-2112-PA-1

**Made by: Robin Alexandra Remollo | 2ECE-D**

The content of this repository contains the Programming Assignment 1 for our course "Advance Computer Programming" this S.Y. 2026-2027. This project covers three python problems pertaining to Module 1 - Base Computing with Python.

# **1. Word Rotation Problem**

Create a function named `rotate_word()` that accepts a non-empty string. Move the first character of the string to the end while keeping all remaining characters in their original order. Preserve the capitalization of every character.

Example: `rotate_word("python")` --> "ythonp"

The following methods were used in this problem:
- `text[1:]` : This uses string slicing to extract all characters from index 1 to the end of the string, the last character.
- `text[0]` : This accessed and extracts the first character of the string located in index 0.
- `+` : The string concatenation operator combines `text[1:]` with `text[0]` to form one string.
