# Regex Tutorial: Matching an Email

## Introduction

This tutorial aims to break down the regular expression used for matching email addresses. By the end of this guide, you'll understand the various components of this regex and how they contribute to accurately identifying valid email addresses.

## Summary

The regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is designed to match most standard email formats. It looks for a sequence of characters before and after the `@` symbol, ensuring there's a domain and a top-level domain.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)

## Regex Components

### Anchors
Anchors are used to ensure the match is made at the start `^` and end `$` of a string. In our regex, `^` ensures the string starts with the pattern, and `$` ensures it ends with the pattern.

### Quantifiers
Quantifiers specify how many instances of a character or group must be present for a match. In our email regex, the `+` quantifier ensures that one or more characters of the preceding type are present.

### Character Classes
Character classes allow matching one character from a specific set. The class `[a-z0-9_\.-]` allows any lowercase letter, digit, underscore, dot, or hyphen. Likewise, `[a-z\.]` matches any lowercase letter or dot.

### Grouping and Capturing
Parentheses `()` are used for grouping and capturing. Each part in parentheses is a captured group. In our regex:
1. `([a-z0-9_\.-]+)` captures the username of the email.
2. `([\da-z\.-]+)` captures the domain.
3. `([a-z\.]{2,6})` captures the top-level domain.

## Author

Victor Marczyk - I'm a coding enthusiast passionate about regular expressions. [Check out my GitHub profile](https://github.com/marczykv).
