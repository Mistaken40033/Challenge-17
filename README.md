#### REGEX Tutorial

Introductory paragraph (Challenge #17)

#### Summary

In this tutorial, we will delve into the world of Regular Expressions (regex), a powerful tool for matching patterns in text. We will explore various components of regex, such as anchors, quantifiers, character classes, and more. By the end of this tutorial, you will have a solid understanding of how to construct and use regex patterns effectively. Here is an example of a regex pattern we will discuss:

```regex
^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}$
```

This pattern is used to match email addresses.

#### Table of Contents

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

#### Regex Components

#### Anchors

Anchors are special characters that specify the position of a match within the text. The two primary anchors are `^` and `$`. The `^` anchor asserts that the match must start at the beginning of the string, while the `$` anchor asserts that the match must end at the end of the string.

Example:
```regex
^hello
```
This pattern matches any string that starts with "hello".

#### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. The common quantifiers are `*`, `+`, `?`, and `{n,m}`.

Example:
```regex
a{2,4}
```
This pattern matches "aa", "aaa", or "aaaa".

#### OR Operator

The OR operator, represented by `|`, allows for matching either the expression before or the expression after the operator.

Example:
```regex
cat|dog
```
This pattern matches either "cat" or "dog".

#### Character Classes

Character classes match any one of a set of characters. They are defined using square brackets `[]`.

Example:
```regex
[aeiou]
```
This pattern matches any vowel.

#### Flags

Flags are optional parameters that can change the behavior of the regex engine. Some common flags include `i` for case-insensitive matching, `g` for global matching, and `m` for multiline matching.

Example:
```regex
/hello/i
```
This pattern matches "hello" in a case-insensitive manner.

#### Grouping and Capturing

Parentheses `()` are used for grouping parts of a pattern and capturing the matched text.

Example:
```regex
(bat|ball)
```
This pattern matches either "bat" or "ball".

#### Bracket Expressions

Bracket expressions match any single character contained within the brackets.

Example:
```regex
[0-9]
```
This pattern matches any digit.

#### Greedy and Lazy Match

By default, quantifiers are greedy, meaning they match as much text as possible. Appending a `?` to a quantifier makes it lazy, matching as little text as possible.

Example:
```regex
a.*?b
```
This pattern matches the smallest string starting with "a" and ending with "b".

#### Boundaries

Boundaries, such as `\b`, assert the position between a word and a non-word character.

Example:
```regex
\bword\b
```
This pattern matches "word" as a whole word.

#### Back-references

Back-references refer to previously captured groups within the same pattern using `\1`, `\2`, etc.

Example:
```regex
(\w+)\s\1
```
This pattern matches repeated words.

#### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow matching a pattern only if it is (or isn't) followed or preceded by another pattern.

Example:
```regex
\w+(?=\d)
```
This pattern matches a word followed by a digit.

##### Author

This tutorial was written by [Erica](https://github.com/Mistaken40033), a regex enthusiast and software developer. You can find more of my work on my github (https://github.com/Mistaken40033).