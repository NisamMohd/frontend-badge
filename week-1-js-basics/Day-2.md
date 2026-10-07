## Day-2

### Js String methods
    • split
    • slice
        slice() is a built-in method that extracts a section of a string (or array) and returns it as a new value, without modifying the original. It exists on both String.prototype and Array.prototype, and interviewers often ask about both.

    • substring

    • substr
        substr() is a built-in string method that extracts a portion of a string by specifying a start index and a length (number of characters), and returns it as a new string without modifying the original.

    • toLowerCase
        toLowerCase() is a built-in string method that converts all characters in a string to their lowercase equivalents and returns the result as a new string. Because strings are immutable, the original string is never changed.

    • concat
        concat() is a built-in method that joins two or more values together and returns a new string (or new array), without modifying the originals.

    • charAt
        charAt() is a built-in string method that returns the character at a given index as a new one-character string. Strings are immutable and zero-indexed, so the original is never changed and the first character is at index 0

    • replace
        replace() is a built-in string method that searches a string for a pattern (a substring or a regular expression) and returns a new string in which the match is replaced by a replacement (a string or a function). Because strings are immutable, the original is never changed

    • trim
        trim() is a built-in string method that removes whitespace from both ends of a string and returns the result as a new string. Whitespace in the middle of the string is left alone. Because strings are immutable, the original is never changed.

    • padStart()
        padStart() is a built-in string method that pads the beginning (left side) of a string with another string, repeated as many times as needed, until the result reaches a target length. It returns a new string. Because strings are immutable, the original is never changed.

### Js String Search methods
    • indexOf()
        indexOf() is a built-in string method that searches a string from left to right and returns the index of the first occurrence of a given substring. It returns -1 if the substring is not found.

    • lastIndexOf()
        lastIndexOf() searches from right to left and returns the index of the last occurrence of a given substring. It also returns -1 if not found.

    • search()
        search() is a built-in string method that tests a string against a regular expression and returns the index of the first match, or -1 if there is no match. It never modifies the original string (strings are immutable) and always returns a number.

    • match()
        match() is a built-in string method that tests a string against a regular expression and returns the matched text (with details), or null if there is no match. It never modifies the original string (strings are immutable).

        What it returns depends on whether the regex has the g (global) flag:

    • includes()    
        includes() is a built-in string method that checks whether a string contains a given substring and returns a boolean: true if found, false if not. It never modifies the original string (strings are immutable) and is case-sensitive.

    • startsWith()
        startsWith() is a built-in string method that checks whether a string begins with a given substring and returns a boolean: true if it does, false if not. It never modifies the original string (strings are immutable) and is case-sensitive.


### Template literals
    A template literal is a string literal delimited by backticks (`) instead of quotes. It supports embedded expressions written as ${expression}, multi-line strings without escape characters, and tagged templates, where a function processes the literal. Template literals were introduced in ES2015 (ES6).