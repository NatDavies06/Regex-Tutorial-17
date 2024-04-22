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
