# Regular Expression for Email Tutorial

In this tutorial I will help you to understand the regex for email.

## Summary

A regular expression is a sequence of characters that specifies a match pattern in text. This a regex for an email address.

      /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

I will be explaining the parts of this regex, what they are and what they mean.

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

Regexes are composed of several different components that work together to define a search pattern.
The most common components include anchors, character classes, quantifiers, and alternation.

### Anchors

The anchors used in this regex expression for matching an email are ^ , which indicates the beginning
of the string and $ to indicate the ending of the string.

### Quantifiers

Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com.
Another quantifier for this regex includes {2,6} , which will allow a match range of 2-6 characters for the character set of [a-z\.].

### OR Operator

The regex OR operator is (|). It is not used in this pattern.

### Character Classes

In the context of regular expressions, a character class is a set of characters enclosed within square brackets. It specifies the
characters that will successfully match a single character from a given input string.
Here are the character classes used in the email regex pattern.
  
    [a-z0-9_\.-]
  
    [\da-z\.-]
  
    [a-z\.]

### Flags

A regular expression consists of a pattern and optional flags: g , i , m , u , s , y. There are no flags used in this email regex pattern.

### Grouping and Capturing

 Parentheses group the regex between them. They capture the text matched by the regex inside them into a numbered group that can be
 reused with a numbered backreference. They allow you to apply regex operators to the entire grouped regex.
 Here are the groupings used in the email regex pattern.

    ([a-z0-9_\.-]+)

    ([\da-z\.-]+)

    ([a-z\.]{2,6})

### Bracket Expressions

A bracket expression (an expression enclosed in square brackets, "[]" ) is an RE that shall match a specific set of single characters,
and may match a specific set of multi-character collating elements, based on the non-empty set of list expressions contained in the
bracket expression.
The bracket expressions used on our email regex pattern are as follows

    [a-z0-9_\.-]

    [\da-z\.-]

    [a-z\.]

### Greedy and Lazy Match

Greedy matching is the default behavior of regular expressions, where the regular expression engine will try to match as much text
as possible. In contrast, non-greedy matching, also known as lazy matching, tries to match as little text as possible.

### Boundaries

Boundary markers such as ^ and $ allow you to anchor the regex pattern to the beginning and end of the line (or string depending
on which flags you use) respectively. This means that when you want to match a literal ^ or $ , you need to escape these special
characters with a backslash.
The boundaries on our email regex pattern are

    /^

    $/

### Back-references

A backreference is a way to match the same text as previously matched by a capturing group. Capturing groups count from 1,
so the first capturing group's result can be referenced with \1 , the second with \2 , and so on. \0 is a character escape for
the NUL character.

### Look-ahead and Look-behind

For matching a pattern that is preceded and/or followed by another one are used the lookaround syntaxes. Lookahead is useful
for matching something depending on the context after it, and lookbehind- the context before it.

## Author

Eric is a Edx Bootcamp Student through the University of Texas Austin.

GitHub username: esbev

GitHub profile: https://github.com/esbev