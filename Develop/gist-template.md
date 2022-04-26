# Email Search, REGEX Expression

Regex stands for regular expression. These are expressions that are used to match patterns in strings. They are made up of a series of characters that define the pattern. This tutorial is a Regex covering user input validation, specifically, an email address.

## Summary

Regex is a powerful tool that can be used to validate user input. It improves efficiency and helps maintain our code. For instance if we want to validate a user's email address, we can use regex to check if the email address is valid. There are many regex patterns that can be used to validate user input. Below will outline the code we use to validate an email address:

REGEX_EMAIL = 
<h3>/^[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$/</h3>

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Author](#author)

## Regex Components
REGEX is made up of different components as you will see below.Each of these components target specific parts of the string. The first and the last character of the regex are the delimiters. REGEX uses / at the beginning and end of the regex to define the content that will target speciific attributes of the search criteria. The / characters are not of the targeted criteria, just what is inside of them. 

### Anchors 
The first character, the caret (^), is used to indicate that the regex will start at the beginning of the string. The last character, the dollar sign ($) is used to indicate that the regex will end at the end of the string.

REGEX_EMAIL = 
<h3>/^[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$/</h3>

### Quantifiers
The (+) is used to indicate that the regex will match one or more of the characters in the regex. The (*) is used to indicate that the regex will match zero or more of the characters in the regex. The (?) is used to indicate that the regex will match zero or one of the characters in the regex. An example of a quantifier is the following: /[a-zA-Z0-9]{3,}/.

The quantifier {0, 61} indicates that the regex will match between 0 and 61 characters. The [a-zA-Z0-9] indicates that the regex will match any of the characters in the range a-z, A-Z, or 0-9.

### Character Classes
The first character class instance is: [a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-] which allows information to be matched in the range a-z, A-Z, 0-9, ., !, #, $, %, &, ', *, +, /, =, ?, ^, _, `, {, |, }, ~, and -. 
The second class instance is: [a-zA-Z0-9] which allows information to be matched in the range a-z, A-Z, 0-9. Only allowing up to 61 characters.
The last clas is a range of characters: [a-zA-Z0-9-] which allows information to be matched in the range a-z, A-Z, 0-9, and -.

Simply put, a character class is a special character that denotes a predefined set of characters. 

### Flags
There are flags that can be used to modify the regex. The first flag is the i flag which indicates that the regex will be case insensitive. The second flag is the m flag which indicates that the regex will match across multiple lines. The third flag is the s flag which indicates that the regex will match the entire string.

### Grouping and Capturing
A group in regex is a set of characters that are establishing a pattern. In the email example the groups are the username, the domain, and the top level domain.

### Bracket Expressions
The bracket expressions are used to group a set of characters together. These groups can be matching or non-matching. Similar to the character classes, the [] expressions can be used to match a set of characters.



## Author

My name is Mitch McKinney and I have been in banking for 10 years. I have always been interested in technology, how it is built and how it communicates. I have decided to take my career down a new path and become a software developer.

My gitHub account: https://github.com/mgmckinn
Email: mgmckinn2325@me.com




