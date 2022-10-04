# REGEX TUTORIAL

The purpose of this tutorial is to further explain the details and specifics of regex. Regular expressions or regex are extremely helpful in extracting information. 
## Summary

Regex is a string of text that lets you create patterns that help locate, manage, and match text.

Matching a URL – /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors belong to the family of the regex tokens that don't match any characters, but that assert something about the string of the matching process.

- "^" Start of string, or start of line in multi-line pattern: example- /^(https?:\/\/)
- "$" matches the end of the string: example- ([\/\w \.-]*)*\/?$/

### Quantifiers
Quantifiers specity how many instances of a character, group, or character class must be present in the input for a match to be found. 
- "*" Matches 0 or more
- "?" 0 or 1
- "+" matches 1 or more

With this knowledge we can take a look at our code and see that part of our example code is ([a-z\.]{2,6}), will match any string holding a-z.



### OR Operator
You can use the | operator (logical OR) to match characters or expression of either the left or right of the | operator. 


### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
