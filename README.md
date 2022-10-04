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

- Example const a = 3;
const b = -2;

console.log(a > 0 || b > 0);
// output: true



### Character Classes
In the context of regular expressions, a character class is a set of characters enclosed within square brackets. It specifies the characters that will successfully match a single character from a given input string.

\s = White space
\S = Not white space
\d = Digit
\D = Not digit
\w = Word
\W = Not word


### Flags
A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way. A flag is denoted using a single lowercase alphabetic character.

- Examples "g, m, i, s, y, and u"

- g, Global, Makes the expression search for all occurrences.
- m, Multiline, Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
- i, Ignore Casing, Makes the expression search case-insensitively.
- s, Dot All, Makes the wild character . match newlines as well.
- y, Sticky, Makes the expression start its searching from the index indicated in its lastIndex property.
- u, Unicode, Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
