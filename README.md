# String Methods Cheat Sheet

This repository contains a Python notebook documenting various string methods. Each method is explained along with examples for better understanding.

## Author
- [Amirreza Jahantab](https://github.com/amirjahantab/)

## Basic Methods
- `str.capitalize()`: Capitalizes the first character of the string.
    ```python
    s = "hello"
    print(s.capitalize())  # Output: "Hello"
    ```
- `str.lower()`: Converts all characters to lowercase.
    ```python
    s = "HELLO"
    print(s.lower())  # Output: "hello"
    ```
- `str.upper()`: Converts all characters to uppercase.
    ```python
    s = "hello"
    print(s.upper())  # Output: "HELLO"
    ```
- `str.title()`: Converts the first character of each word to uppercase.
    ```python
    s = "hello world"
    print(s.title())  # Output: "Hello World"
    ```
- `str.swapcase()`: Swaps the case of all characters.
    ```python
    s = "Hello"
    print(s.swapcase())  # Output: "hELLO"
    ```
- `str.casefold()`: Converts to lowercase, suitable for caseless comparisons.
    ```python
    s = "HELLO"
    print(s.casefold())  # Output: "hello"
    ```

## Query Methods
- `str.islower()`: Checks if all characters are lowercase.
    ```python
    s = "hello"
    print(s.islower())  # Output: True
    ```
- `str.isupper()`: Checks if all characters are uppercase.
    ```python
    s = "HELLO"
    print(s.isupper())  # Output: True
    ```
- `str.istitle()`: Checks if the string is title-cased.
    ```python
    s = "Hello World"
    print(s.istitle())  # Output: True
    ```
- `str.isalpha()`: Checks if all characters are alphabetic.
    ```python
    s = "Hello"
    print(s.isalpha())  # Output: True
    ```
- `str.isdigit()`: Checks if all characters are digits.
    ```python
    s = "123"
    print(s.isdigit())  # Output: True
    ```
- `str.isalnum()`: Checks if all characters are alphanumeric.
    ```python
    s = "Hello123"
    s1 = "Hello123!"
    print(s.isalnum())  # Output: True
    print(s1.isalnum())  # Output: False
    ```
- `str.isnumeric()`: Checks if all characters are numeric.
    ```python
    s = "1230"
    print(s.isnumeric())  # Output: True
    ```
- `str.isdecimal()`: Checks if all characters are decimal characters.
    ```python
    s = "123"
    print(s.isdecimal())  # Output: True
    ```
- `str.isspace()`: Checks if all characters are whitespace.
    ```python
    s = " "
    print(s.isspace())  # Output: True
    ```
- `str.startswith(prefix[, start[, end]])`: Checks if the string starts with the specified prefix.
    ```python
    s = "hello"
    print(s.startswith("he"))  # Output: True
    ```
- `str.endswith(suffix[, start[, end]])`: Checks if the string ends with the specified suffix.
    ```python
    s = "hello"
    print(s.endswith("lo"))  # Output: True
    ```

## Modification Methods
- `str.strip([chars])`: Removes leading and trailing characters (default is whitespace).
    ```python
    s = "  hello  "
    print(s.strip())  # Output: "hello"
    ```
- `str.lstrip([chars])`: Removes leading characters (default is whitespace).
    ```python
    s = "  hello  "
    print(s.lstrip())  # Output: "hello  "
    ```
- `str.rstrip([chars])`: Removes trailing characters (default is whitespace).
    ```python
    s = "  hello  "
    print(s.rstrip())  # Output: "  hello"
    ```
- `str.replace(old, new[, count])`: Replaces occurrences of a substring.
    ```python
    s = "hello world"
    print(s.replace("world", "there"))  # Output: "hello there"
    ```
- `str.join(iterable)`: Joins elements of an iterable with the string as a separator.
    ```python
    print(", ".join(["a", "b", "c"]))  # Output: "a, b, c"
    ```
- `str.split(sep=None, maxsplit=-1)`: Splits the string by the specified separator.
    ```python
    s = "hello world"
    print(s.split())  # Output: ["hello", "world"]
    ```
- `str.rsplit(sep=None, maxsplit=-1)`: Splits the string by the specified separator, starting from the right.
    ```python
    s = "hello world"
    print(s.rsplit())  # Output: ["hello", "world"]
    ```
- `str.splitlines([keepends])`: Splits the string at line breaks.
    ```python
    s = "hello\nworld"
    print(s.splitlines())  # Output: ["hello", "world"]
    ```
- `str.partition(sep)`: Splits the string at the first occurrence of the separator.
    ```python
    s = "hello world"
    print(s.partition(" "))  # Output: ("hello", " ", "world")
    ```
- `str.rpartition(sep)`: Splits the string at the last occurrence of the separator.
    ```python
    s = "hello world"
    print(s.rpartition(" "))  # Output: ("hello", " ", "world")
    ```
- `str.expandtabs(tabsize=8)`: Expands tabs into spaces.
    ```python
    s = "hello\tworld"
    print(s.expandtabs(4))  # Output: "hello   world"
    ```

## Search Methods
- `str.find(sub[, start[, end]])`: Finds the lowest index of the substring.
    ```python
    s = "hello"
    print(s.find("e"))  # Output: 1
    ```
- `str.rfind(sub[, start[, end]])`: Finds the highest index of the substring.
    ```python
    s = "hello"
    print(s.rfind("l"))  # Output: 3
    ```
- `str.index(sub[, start[, end]])`: Finds the lowest index of the substring, raises an error if not found.
    ```python
    s = "hello"
    print(s.index("e"))  # Output: 1
    ```
- `str.rindex(sub[, start[, end]])`: Finds the highest index of the substring, raises an error if not found.
    ```python
    s = "hello"
    print(s.rindex("l"))  # Output: 3
    ```
- `str.count(sub[, start[, end]])`: Counts occurrences of a substring.
    ```python
   

 s = "hello"
    print(s.count("l"))  # Output: 2
    ```

## Formatting Methods
- `str.center(width[, fillchar])`: Centers the string in a field of the given width.
    ```python
    s = "hello"
    print(s.center(10))  # Output: "  hello   "
    ```
- `str.ljust(width[, fillchar])`: Left-justifies the string in a field of the given width.
    ```python
    s = "hello"
    print(s.ljust(10))  # Output: "hello     "
    ```
- `str.rjust(width[, fillchar])`: Right-justifies the string in a field of the given width.
    ```python
    s = "hello"
    print(s.rjust(10))  # Output: "     hello"
    ```
- `str.zfill(width)`: Pads the string with zeros on the left, to fill the given width.
    ```python
    s = "42"
    print(s.zfill(5))  # Output: "00042"
    ```
- `str.format(*args, **kwargs)`: Performs a string formatting operation.
    ```python
    print("{name} is {age} years old".format(name="Alice", age=30))  # Output: "Alice is 30 years old"
    ```
- `str.format_map(mapping)`: Formats the string using a mapping.
    ```python
    print("{name} is {age} years old".format_map({"name": "Alice", "age": 30}))  # Output: "Alice is 30 years old"
    ```

## Encoding and Decoding Methods
- `str.encode(encoding="utf-8", errors="strict")`: Encodes the string to bytes using the specified encoding.
    ```python
    s = "hello"
    print(s.encode())  # Output: b'hello'
    ```
- `str.decode(encoding="utf-8", errors="strict")`: Decodes the bytes to a string using the specified encoding.
    ```python
    b = b'hello'
    print(b.decode())  # Output: "hello"
    ```
