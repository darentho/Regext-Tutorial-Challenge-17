# Title (replace with your title)

REGEX TUTORIAL: REGULAR EXPRESSIONS THAT MATCH A URL.

## Summary

A Regex proves useful in matching a URL in order to locate special text patterns. Short for regular expression, a regex is a string of text that lets you create patterns that help match, locate, and manage text. URL regular expressions can be used to verify if a string has a valid URL format as well as to extract an URL from a string.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Anchors are used at the beginning and end of searches to check if a string fully matches a pattern, although they themselves do not match characters. They strictly affirm a string matches a location. Anchors will create parameters.

Use the ^ anchor to match the beginning of the text.
Use the $ anchor to match the end of the text.

### Quantifiers

Quantifiers will measure and set the limit on the the number of characters that we are wanting to match in our Regex: + searches the pattern one or more times, ? searches the pattern zero or one time, \* searches the pattern zero or more times. https? for= example. The ? will make the preceeding itme optional.

### Grouping Constructs

Capturing Group is a part of a pattern that can be enclosed in a parentheses () and is a way to treat multiple characters as one unit. The example expression has many groupings such as: https?:\/\/ which is looking for the http(s),(www\.)?[\d-a-zA-Z0-9@:%._\+~#=] which will look for initial domain, [a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=] looks for top level domain, and \*) file paths.

### Bracket Expressions

is a matching or non-matching list expression and consists of one or more expressions that will be found in square brackets []. It represents a special character class and is a quantified rule providing range construct. They adapt to a users or applications locale. A bracket expression is either a matching list expression or a non-matching list expression. It consists of one or more expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions. The <right-square-bracket> ( ']' ) shall lose its special meaning and represent itself in a bracket expression if it occurs first in the list (after an initial <circumflex> ( '^' ), if any). Otherwise, it shall terminate the bracket expression, unless it appears in a collating symbol (such as "[.].]" ) or is the ending <right-square-bracket> for a collating symbol, equivalence class, or character class. The special characters '.', '\*', '[', and '\\' ( <period>, <asterisk>, <left-square-bracket>, and <backslash>, respectively) shall lose their special meaning within a bracket expression.

### Character Classes

A character class is the set of characters that could occur in a string.
The \d character class in the above code is looking for any digits, whereas a \D looks for non-digits, \s searches for space symbols, tab and newlines, \S looks for all but \s, . any characters with the regex 's' flag, while the included \w character is looking for an alphanumeric character.

### The OR Operator

The purpose of an OR operator is to match the characters on the left or right of the operator, essentially serving as an or, as in and/or. Using the | as in m|M would match either m or an M from the string. If we had used https?:\/\/(www\.)?[\d-a|A it would search or a OR A.

### Flags

Regular expressions may have flags that affect the search.

There are only 6 of them in JavaScript:

i
With this flag the search is case-insensitive: no difference between A and a (see the example below).
g
With this flag the search looks for all matches, without it – only the first match is returned.
m
Multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m").
s
Enables “dotall” mode, that allows a dot . to match newline character \n (covered in the chapter Character classes).
u
Enables full Unicode support. The flag enables correct processing of surrogate pairs. More about that in the chapter Unicode: flag "u" and class \p{...}.
y
“Sticky” mode: searching at the exact position in the text (covered in the chapter Sticky flag "y", searching at position)

### Character Escapes

The characters listed above have special meanings in regex. To match these characters, we need to prepend it with a backslash (\), known as escape sequence. For examples, \+ matches "+"; \[ matches "["; and \. matches ".".

Regex also recognizes common escape sequences such as \n for newline, \t for tab, \r for carriage-return, \nnn for a up to 3-digit octal number, \xhh for a two-digit hex code, \uhhhh for a 4-digit Unicode, \uhhhhhhhh for a 8-digit Unicode.
The \ is known as the escape code, which restore the original literal meaning of the following character. Similarly, \* , + , ? (occurrence indicators), ^ , $ (position anchors) have special meaning in regex. You need to use an escape code to match with these characters.

## Author

Alberto Monroy is a Tech de Monterrey Bootcamp Student aspiring to be a Full-Stack web developer. His current place of residence is Mexico City.

image.png[Alberto’s Github](https://github.com/darentho)
image.png[Alberto's Linkedin](https://www.linkedin.com/in/alberto-monroy-b734a8150/)
📩[Alberto's Email](mailto:firewind3882@gmail.com)
