# regex_tutorial

The purpose of this assignment is to explain how to use a Regex if you were a complete beginner.


## Summary

The regular expression that I am going to be explaining today is this:

`/^[a-z0-9_-]{3,16}$/`

This is the regular expression used for matching a Username. 



## Table of Contents

- [Gist](#gist)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Resources](#resources)



## Regex Components



### Anchors

    The characters `^` and `$` are the anchors that are being used in this regular expression.

    The `^` symbol is what begins a string. Everything that follows this are the parameters that are being searched with this regular expression

    The `$` symbol is what ends the string started by the `^` symbol. 



### Bracket Expressions

    The bracket expression, `[]` lets you match with whatever character you put in them. Hyphens, `-`, are often used to help us refine our search. In our example we see `[a-z]`, which simply means that we are looking for any characters between a through z. 



### Quantifiers

This regular expression contains multiple quantifiers.

    The most common ones are `+`, `?`, `*`, `{}`.

    The `+` quantifier lets you match with many in a row but match with at least one.

    The `?` quantifier basically whatever its in front of it, is optional.

    The `*` quantifier essentially does the `+` and `?` in the same time.

    The `{}` quantifier you can put a min and max number of how large you want something.




### Grouping Constructs

    The expression being used also contains a grouping construct. These are displayed by using `()`, anything the parentheses are their own group and act upon themselves.


### Character Classes

    "A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match. We've actually already discussed some character classes. The bracket expressions outlined previously, including positive and negative character groups, are considered character classes."



### The OR Operator

    The (|) character basically acts a boolean  'or'  and matches the expression before it or after it.

    For example, if you want to look for the letter t and T at the same time, you write it as (t|T).  

### Flags

    Flags help specify your search. "Note that the flags are an integral part of a regular expression. They cannot be added or removed later."

        - g—Global search: the regex should be tested against all possible matches in a string.

        - i—Case-insensitive search: case should be ignored while attempting a match in a string

        - m—Multi-line search: a multi-line input string should be treated as multiple lines"
        



### Character Escapes

    The (/)  makes characters literal instead of special. It basically cancels out whatever its in front of it.

    For example: (/.) will treat that period as a normal period instead of  the (.) character type.

## Gist

[Link to my Gist](https://gist.github.com/GustavoTijerino1/f9f411844e94cd4c687c9aebf5f129c5)

## Author

Gustavo Tijerino

[Link to my Github](https://github.com/GustavoTijerino1/regex_tutorial)

## Credits

Andrew Anderson


## Resources

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#examples

https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial

https://youtu.be/rhzKDrUiJVk
