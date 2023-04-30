# Regular Expression

Regular expressions also go by regex for short is a sequence of characters that define a search patter. Programmers are able to use this tool for text processing to search, manipulate, and validate text data. Regular expressions can be used to match patterns within strings, search for specific characters or words, or validate input data for a variety of use cases such as form validation or data parsing.

## Summary

Match any character in the range of a-z
regex = r'[a-z]'
text = "The quick brown fox jumps over the lazy dog."
match = re.findall(regex, text)
print(match)
Output: ['h', 'e', 'q', 'u', 'i', 'c', 'k', 'b', 'r', 'o', 'w', 'n', 'f', 'o', 'x', 'j', 'u', 'm', 'p', 's', 'o', 'v', 'e', 'r', 't', 'h', 'e', 'l', 'a', 'z', 'y', 'd', 'o', 'g']

Match any character that is not a digit or a whitespace character
regex = r'[^\d\s]'
text = "The number 42 is greater than 3.1415."
match = re.findall(regex, text)
print(match)
 Output: ['T', 'h', 'e', 'n', 'u', 'm', 'b', 'e', 'r', 'i', 's', 'g', 'r', 'e', 'a', 't', 'e', 'r', 't', 'h', 'a', 'n', '.', '.']

In the first example, the regex [a-z] matches any lowercase letter from a to z in the given text. The re.findall() function is used to find all non-overlapping matches of the regex pattern in the text.

In the second example, the regex [^\d\s] matches any character that is not a digit (\d) or a whitespace character (\s). The ^ inside the square brackets means to match any character not in the specified range.


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
These are characters used to define the start and end of a line or string, such as ^ for the start of a line and $ for the end of a line.

### Quantifiers
These are used to define how many times a character or group can occur, such as ? for zero or one occurrence, * for zero or more occurrences, and + for one or more occurrences.

### OR Operator
This operator is represented by the vertical bar | and is used to specify a set of alternatives, where one of the alternatives must be matched.

### Character Classes
These are used to match specific sets of characters, such as digits \d, whitespace characters \s, or any character except newline characters with '.'.

### Flags
These are used to change the behavior of a regular expression, such as making it case-insensitive with the i flag or to treat the input as a multiline string with the m flag.

### Grouping and Capturing
These are used to group characters or expressions together and capture the matched text. They are represented by parentheses ( ).

### Bracket Expressions
These are used to match a range or set of characters, where the characters are enclosed in square brackets [ ].

### Greedy and Lazy Match
These are used to specify how many characters should be matched by a quantifier, such as whether it should match as many as possible (greedy) or as few as possible (lazy).

### Boundaries
These are used to match characters at the beginning or end of a word, or to match characters that are not surrounded by word characters.

### Back-references
These are used to match the same text that was previously matched by a capturing group, such as \1 to match the same text as the first capturing group.

### Look-ahead and Look-behind
These are used to match text that is followed by or preceded by specific characters or expressions, without including the characters or expressions in the match.

## Author

I am a full stack software developer.some examples of me work are here in [BaldOracle GitHub Profile](https://github.com/BaldOracle)