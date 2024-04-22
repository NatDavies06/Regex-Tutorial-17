# Regex Turtorial

Regex is a tool for pattern matching  within a string in JavaScript. I aim to explain the functionality of a regex pattern by breaking down each component and its purpose.

## Summary

In this turorial I'll dive into the regex pattern for matching email adresses:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This pattern is made to validate email adresses entered by a user.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

Anchors make sure the regex pattern checks right at the beggining and end of the text. In the email, the `^` symbol is the start, while the `$` symbol is the end.

`/^...$/`

Example:

`^abc@example.com$ matches the whole "abc@example.com".`

### Quantifiers

Quantifiers tell us how many times preceding elements should appear. In our email regex `{2,6}` tell us the domain extension should be 2 to 6 characters long.

`/{2,6}/`

Example:

`'example.com' matches because it's 11 characters long, fitting in our range.`

### OR Operator

OR operator (`i`) allows alternative matches. In the email regex, it lets the domain extension be either 6 characters or 3 characters.

`/(abc|def)/`

Example: 

`abc matches the OR condition, because it's one of the specified alternatives.`

### Character Classes

Character classes define a set of character matches. In our regex email, `[a-z0-9_\.-]` matches lowercase letters, digits, underscores, hyphens nad dots in the local part of the email.

Example:


### Grouping and Capturing

Parentheses `()` are used for grouping and catching substrings. In our email regex, they capture the local part, domain and domain extension seperately.

`/(abc)/`

For instance:

`abc is captured as a substring for later processing.`


### Bracket Expressions

Bracket expressions `[...]` match any character within the set. In our email regex `[\da-z\.-]` matches digits, lower case letters, dots and hyphens in the domain.

`[\da-z\.-]`

Example:

5 matchs the bracket expression, becasue it's a digit.

## Author

My name is Nathan Davis, I'm currently a enrolled in the University of Minesota Coding Bootcamp. Can't wait to see what the future holds.

Github: 
