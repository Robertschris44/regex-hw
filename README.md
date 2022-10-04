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

- \s = White space
- \S = Not white space
- \d = Digit
- \D = Not digit
- \w = Word
- \W = Not word


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
- Groups group multiple patterns as a whole, and capturing groups provide extra submatch information when using a regular expression pattern to match against a string.

- Parentheses group the regex between them. They capture the text matched by the regex inside them into a numbered group that can be reused with a numbered backreference. They allow you to apply regex operators to the entire grouped regex.

- Example in our sample code above: the following is the second group "([\da-z\.-]+)", you can tell this because it is separated from the first group by a "?" and a different set of parenthesis. 

### Bracket Expressions
Bracket expressions can be used to match a single character or collating element. Each set a bracket expressions can include special characters,letters, and numbers. Examples below:
- [abcd]
- [a-d]
- a-z for lower case letters
- A-Z for upper case letters
- _ Underscores
- 0-9 for numberical digits to 0-9

In our example ([a-z\.]{2,6}), you can see a-z present in the bracket.

### Greedy and Lazy Match
Greedy and lazy are quantifiers.

- Lazy means matching the shortest possible string. Examples: "*?", "+?", "??"
- Greedy means match longest possible stings. Examples: "*", "+", "?"

### Boundaries
- The (\b) is an anchor like the caret (^) and the dollar sign ($). 
- It matches a position that is called a “word boundary”. 
- The word boundary match is zero-length.
Example below:

The following matches a 4-digit number surrounded by characters from a different \w
console.log('ES 2022'.match(/\b\d\d\d\d\b/)); Output: "2022"



### Back-references
- Lets say you want to match a pair of opening and closing HTML tags, and the text in between. 
Here’s how: <([A-Z][A-Z0-9]*)\b[^>]*>.*?</\1>. This regex contains only one pair of parentheses, which capture the string matched by [A-Z][A-Z0-9]*. 
- Click [https://www.regular-expressions.info/backref.html] for further details.

- Backreferences match the same text as previously matched by a capturing group.
- back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are specified with backslash and a single digit 
(e.g. ‘\1’). The part of the regular expression they refer to is called a subexpression, and is designated with parentheses.


### Look-ahead and Look-behind
- Look-ahead and Look-behind match the context before or after the string

- Examples
(?=foo)	Lookahead	Asserts that what immediately follows the current position in the string is foo

(?<=foo)	Lookbehind	Asserts that what immediately precedes the current position in the string is foo

## Author

Christopher Roberts, Student in Full stack development Bootcamp at SMU

- Github [https://github.com/Robertschris44]
