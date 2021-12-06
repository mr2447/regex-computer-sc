# Tutorial: Regex of the email format: 
The purpose of this tutorial is to explain the parts of a regular expression in the email format. This will be a thorough explanation of every aspect of that expression. As needed, it can be used to first understand a search pattern the regex defines.

## Summary
The regex expression this tutorial will discuess is as follow: 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The tutorial will discuss every aspects of this expression from the specific to the general. When appropriate, the tutorial will identify the catogories in which the characters references according to the RegEx Reference page on regexr.com This will aid the understanding of said expression. The topics include but are not limited to character classes, in which characters are selected, anchors, in which positions are identified, escaped characters, in which some characters must be preceeded by, groups, in which patterns are organized, and finally, quantifiers, in which quantities are accounted for. 

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

### Anchors
    Although not an Achor element according to regexr.com, the open and close "/"s must be used to indicate the start and end of any regular expression. Yet, two anchor elements are used in this expression: "^" and "$". "^" matches the beginning of the string while "$" matches the end of the string. When executed, the characters in between "^" and "$" will be read as a string and not a line since the multiline flag is not used in this case. 
### Quantifiers
    Two quantifiers are used in this expression: "+" and "{x,y}". "+" is a quantifier that matches one or more of the preceeding pattern. In the case of the first group of the email expression, it wants at least one character that belongs to the types a-z, or numbers 0-9, or character "_", ".", or "-". In the case of the second group after the @ character, it wants at least one character that belongs to the types any digits 0-9, or any characters a-z, or character "." or "-". Lastly, the "{x,y}" quantifier matches a range for the preceeding pattern. This sets the limit for the letters a-z or "." to 2 to 6 characters in length. 
### OR Operator
    None used 
### Character Classes
    Several character classes are used in this expression. Starting with the first character set "[a-z0-9_\.-]", the set contains characters that belongs to the types a-z, or numbers 0-9, or character "_", ".", or "-" respectively. The next space is occupied by a literal character "@", meaning it has to be this character with no exception. Then comes the second set which includes characters that belongs to the types any digits "\d" 0-9, any letters a-z, or any characters ".", or "-". This is followed by yet another literal character ".". Finally, the third set is comprised of any letters a-z, or character ".". Recall from the Quantifiers section in which the character classes are grouped along side with, those qualifiers will be added to each character sets appropriately (Refer to Quantifiers).
### Flags
    None
### Grouping and Capturing
    This regular expression is group in three groupings, each containing a specific character set and a qualifier. The character sets are organized in square brackets"[]" while the qualifiers are "+" and "{2,6}". Hence, groupings can group multiple patterns together and creates a capture group.
### Bracket Expressions
    Character sets are in bracket expression, the organization of strings in square brackets "[]". It matches any characters in the set. There are three bracket expressions in this example. It allows types of characters to be included in a desired pattern. 
### Greedy and Lazy Match
    None used
### Boundaries
    None used 
### Back-references
    None used
### Look-ahead and Look-behind
    None used
## Author

Marvin is a full stack developer with a full-stack certificate and a B.M and M.M degrees in Muiscal performances. Contact: https://github.com/mr2447
