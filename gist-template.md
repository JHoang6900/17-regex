# Discord Username Regex Explanation by JHoang: 

## Summary

The regex I will be describing is an expression that matches username tags for the popular VoIP and instant messaging social platform, 'Discord.'Discord's allows usernames with a minimum of 3 characters and a  maximum of up to 32 characters, while allowing special characters.
The username then is followed up by a hash `#` and four digits. 

Here is the Discord Regex Expression: 

```
^.{3,32}#[0-9]{4}$/gm
```



- `^` starts at the beginning of the string
- `.` wildcard for any character (except for newline)
- `{3,32}` matches the preceding character (`.`) between 3 and 32 times
- `#` matches the hash symbol literally
- `[0-9]` matches numbers between 0 and 9
- `{4}` matches the preceding character class (`[0-9]`) exactly 4 times
- `$` ends  the position at the end of the string
- `/gm` global and multiline flags are enabled. 

## Table Of Contents: 

- [Discord Username Regex Explanation by JHoang:](#discord-username-regex-explanation-by-jhoang)
  - [Summary](#summary)
  - [Table Of Contents:](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [Grouping Constructs](#grouping-constructs)
    - [Bracket Expressions/Character Classes](#bracket-expressionscharacter-classes)
    - [The OR Operator](#the-or-operator)
    - [Flags](#flags)
    - [Character Escapes](#character-escapes)
  - [Author](#author)

## Regex Components

### Anchors	

- The anchors used in this regex expression are `^` and `$`. 
- The carat `^` is used to match items at the beginning of the string. 
- The dollar sign `$` is used to match items at the end of the string. 

### Quantifiers

- The quantifiers in the regex expressions used are `{3,32}` and `{4}`.
- The `{3,32}` quantifier is used to have a minimum of 3 characters and up to 32 characters, following Discord's username guidelines.
- The `{4}` quantifier is used to match up to four numbers after the hashtag, in accordance to Discord's username tag system.  

### Grouping Constructs

- ​	This regex expression does not need to use capture groups as each match is a singular capture group, encompassing the one's whole username. 

### Bracket Expressions/Character Classes

- From my understanding, bracket expressions are expressions to match character classes. Therefore, I have combined these two. 
- This regex expression uses the `[0-9]` bracket expression to match any numerical digits as any 4 numbers can be used in Discord's naming scheme. 

### The OR Operator

- The need for the OR Operator `|` was not needed in this regex expression.

### Flags

- the `g` and `m` flags are enabled for global and multiline matching.
- the global flag is enabled to scan the entirety of the input. 
- the multiline flag is enabled to scan multiple lines even after the new line character. 

### Character Escapes

- No character escapes were used in this regex expression. 

## Author

JHoang is a student currently attending the University of Utah Coding Bootcamp studying to become a Junior Developer. 
Link to Github Profile: https://github.com/JHoang6900
