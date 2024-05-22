# Understanding the Phone Number Regular Expression
## Phone Number Regex Tutorial

In this tutorial we will be going over regular expressions, or regex for short. Regex are powerful tools for pattern matching in strings, in which we will have a complete break down of in this tutorial.
More specifically we will be breaking down the Phone number regex, a way to match US phone numbers, in hopes that you too can impliment into your own projects and knowledge base.

## Summary

This tutorial will explain the regex pattern used to match US phone numbers in the format (123) 456-7890. 
The regex pattern we'll be examining is:
^\(\d{3}\) \d{3}-\d{4}$
We will cover each component of this regex, explaining how it matches the desired phone number format.

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

Anchors are used to specify the position in the string where the regex should match.
- `^`: Matches the start of the string.
- `$`: Matches the end of the string.
Therefore, in our regex - `^` and `$` - ensure that the entire string must match the pattern (specified within the start and end operators) from start to end.

### Quantifiers

Quantifiers specify how many times a character or group should be matched.
- `{3}`: Matches exactly 3 occurrences of the preceding element.
- `{4}`: Matches exactly 4 occurences of the preceding element.
In our regex:
- `\d{3}`: Matches exactly 3(three) digits.
- `\d{4}`: Matches exactly 4(four) digits.

### OR Operator

The OR operator (`|`) - commonly called `pipe` - allows for matching of one pattern or another. Although not used in this specific regex, it is useful for matching multipole possible patterns.

### Character Classes

Character classes match any one of the caracters in the set.
- `\d`: Matches any digit (equivalent to [0-9]).
- Example: `\d` matches "1" in "123".

### Flags

Flags are used to in modifying the behavior of the regex, such as making it case-insensitive or allowing it to match across multiple lines. This regex does not use any flags.
Since this regex does not used flags or OR operator's we can talk quickly about Literals.

### Literals

Literals are used to match the exact characters specified.
- `\(`: Matches exactly `(`
- `\)`: Matches exactly `)`
These characters are used for grouping in regex, so they need to be escaped with a backslash to be matched literally.
Insert `` for spaces and `-` for hashes to be read literally.

### Grouping and Capturing

Paraentheses `()` are used for grouping parts of the regex and capturing the matched content values.
- `\(\d{3}\)`: Matches exactly three digits enclosed in parentheses.

### Bracket Expressions

Bracket expressions, also known as character classes, match any one character within the brackets. For example, [abc] matches a, b, or c. This regex does not use bracket expressions.

### Greedy and Lazy Match

Greedy matches try to match as much as possible, while lazy matches try to match as little as possible. This regex uses greedy matching, which is the default behavior.

### Boundaries

Boundaries match positions, not characters. Neither of these are used in this regex.
- `\b`: Matches a word boundary.
- `\B`: Matches a non-word boundary.

### Back-references

Back-references allow a previous part of the matched string to be referenced later in the regex. This regex does not use backk-references.

### Look-ahead and Look-behind

Again Look-ahead and look-behind assertions are not used in this regex. But they do allow you to match a pattern only if it is followed or preceded by another pattern.

## Author
*** Max Bonetti ***, a web development student eager to explore and share the ins-and-outs of programming languages and tools. Find out more below!
*** GitHub *** - [GitHub Profile](https://github.com/maxbonetti)
*** Repo Link *** - [Application Repository](https://github.com/maxbonetti/regex-tutorial-app)
*** Pages' Link *** - [Application pages' link]() 
