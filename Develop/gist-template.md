Match an Email - Regex 

Regular expressions can be used to find certain patterns of characters within a string. You can also find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

## Summary
A regular expression is a sequence of characters that defines a search pattern. This is commonly used to find patterns within a string, find/replace characters within a string or validate input. This tutortial will go walk through the components of a regex and how it applies to matching an email. Example /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)




### Anchors
The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers
Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com.
Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].


### Character Classes
The character class in this expression is \d, which matches a single characters that is a digit from 0-9.


### Grouping and Capturing
Regular expressions allow us to not just match text but also to extract information for further processing. This is done by defining groups of characters and capturing them using the special parentheses ( and ) metacharacters. Any subpattern inside a pair of parentheses will be captured as a group. In practice, this can be used to extract information like phone numbers or emails from all sorts of data.

They are useful for creating blocks of patterns, so you can apply repetitions or other modifiers to them as a whole. In the pattern ([a-x]{3}[0-9])+, the + metacharacter is applied to the whole group.

### Bracket Expressions

Bracked expressios for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; [a-z\.] matches any character a-z(case senstive) and the character

### Greedy and Lazy Match
 the two quantifiers regrex includes greedy matches. the first will be + Quantifier, it will match as many times as as needed. Another greedy Quantifier used in this regex is {} when matching `{2,6} for the last capture group

### Boundaries
Boundary markers such as ^ and $ allow you to anchor the regex pattern to the beginning and end of the line (or string depending on which flags you use) respectively. This means that when you want to match a literal ^ or $, you need to escape these special characters with a backslash.


## Author
https://github.com/Dmj22
