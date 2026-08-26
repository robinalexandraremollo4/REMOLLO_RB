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

These methods defined the function `rotate_word(text)` to move the first character of the string to the end of the substring;

```python
def rotate_word(text):
    return text[1:] + text[0]
```

# **2. Username Builder Problem**

Create a function named `make_username()` that accepts two strings: first_name and last_name.
The function must:
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).

Example: `make_username("Ada", "Lovelace")` --> "ada.lovelace"

The following methods were used in this problem:

 - `.lower()` : This is a built-in string method that changes all letters to lowercase.
 - `.replace(" ", "")` : This is a built in string method that removes all the spaces from the string and replaces it with an empty string.
 - `+ "." +`  : This string concatenation operator connects the now modified first name with the period and the last name.

Final Function:

```python
def make_username(first_name, last_name):
    first_name = first_name.lower().replace(" ", "")
    last_name = last_name.lower().replace(" ", "")
    return first_name + "." + last_name
```

# **3. Bookend Swap Problem**

Create a function named swap_bookends() that accepts a list containing at least two elements. Unpack the list into three variables:
a. first – the first element;
b. middle – a list containing everything between the first and last elements; and
c. last – the last element.
Using these variables, return a new list in which the first and last elements have exchanged positions.
The elements in middle must remain in their original order. Do not modify the input list.

Example: `swap_bookends([1, 2, 3, 4, 5, 6])` -> [6, 2, 3, 4, 5, 1]"

The following methods were used in this problem:

- `first, *middle, last = items` : This is extended sequence unpacking that assigns the first element to `first`, the last element to `last`, and gathers all elements in the middle. 
- `last, *middle, first` : This is a technique known as list unpacking that creates a new list by switching the first and last elements while keeping the middle elements stayed put.

  Final Function:

```python
def swap_bookends(items):
    first, *middle, last = items
    return [last, *middle, first]
```

Thank you for reading!

To see the main python program for Progrsmming Assignment 1, click this link [https://github.com/robinalexandraremollo4/REMOLLO_RB](https://github.com/robinalexandraremollo4/REMOLLO_RB/blob/main/%5BREMOLLO_2ECED%5D%20(1).ipynb)

  




