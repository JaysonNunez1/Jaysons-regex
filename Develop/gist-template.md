# Jaysons Regex Tutorial 

# Introduction
In this tutorial, we will learn about regex and how we can use it.Using github gist i will be breaking down and explaing the various components of a regex.
## Summary
Regex, or Regular Expressions, is a sequence of characters that forms a search pattern. It can be used to check if a string contains the specified search pattern. Regex is commonly used for string matching, validation, and extraction.

For this tutorial,i will explain the different components for the following regex that is used to match an email.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
An Anchor component will display the string of characters that are included within the anchors.In the example the ^ character is starting the string of characters and the $ is used to end the string of characters.
### Quantifiers
Quantifiers will put a limit on the amount of characters that can match the regex.In the example the + is being used to connect the user's email name to their email service. 
### OR Operator

### Character Classes
Character classes are a set of defined characters in a regex.In the example the \d causes the regex to match with single digit characters like 0-9
### Flags
Flags are implemented with the characters.
### Grouping and Capturing
A regex will contain many characters inside of it.Parentheses are used to section charcter sets and characters inside of the parentheses.
([a-z0-9_.-]+) is the first subexpression which is the user's email name.
([\da-z.-]+) is the second subexpression which is the user's email service.
([a-z.]{2,6}) is the third subexpression which provides the .com part of the email address.
### Bracket Expressions
Characters within the bracket expressions are characters that will match the regex.These characters are sometimes referred to as the positive character group because these are the characters that will match the regex.
In the first subexpression [a-z0-9_.-] means that the lower case characters a-z and single digit numbers 0-9 are the positive character group.'_', '', '.', and '-' will also be in the positive character group.
### Greedy and Lazy Match
A greedy match will match as many characters as possible. A lazy match will match as few characters as possible.The two '+' characters that are used at the end of the first two subexpressions; ([a-z0-9_.-]+) and ([\da-z.-]+) means a greedy match.
### Boundaries
Boundaries are used to match the beginning and end of a string.
### Back-references
Back-references search for previously matched groups.
### Look-ahead and Look-behind
Look-ahead is used to make the character that immediately follows the look-ahead to be capitalized,while the look-behind is used to make the charcter that immediately follows the look-behind to be lower cased.
## Author
Jayson Nunez Currently enrolled in the full stack coding bootcamp at Columbia University.

Github: https://github.com/JaysonNunez1
