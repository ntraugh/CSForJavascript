# CSForJavascript

This tutorial will teach you how to read a regular expression that matches an email.

## Summary

Regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This regular expression will match our email.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Our ^ anchor lets us know that the current position in the string is the beggining of the string.  The $ anchors the end of the string, so for our example would match the ".com" of our email with no more than 6 characters allowed.

### Quantifiers

The quantifiers specify how many instances of a character should be present in the input. Usually this is a number in curly brackets, in our case it would refer to the {2,6} at the end of the string.

### Grouping Constructs

Grouping constructs are fairly self-explanatory, we are grouping sub groups of the string together to test for them that much easier.  In our example we can see that we have certain parts of our email grouped together. The first being the "name" of the email, the second after the "@" symbol, and the third to match the ".com".

### Bracket Expressions

We place characters inside of the brackets that we want to match or look for in our regex.  In our example we use a hyphen to define anything from a-z as well as 0-9 and we account for underscores and forward slashes.

### Character Classes

A character class is essentially anything we put inside of those square brackets.  The character class will match whatever we put into the square brackets. In our regular expression we are matching a through z as well as the numbers 0 through 9. 

### The OR Operator

The OR expression is just like the one we use in javascript, except instead of two bars we use one like | . We don't need to use an OR operator in our email verification though. 


### Character Escapes

In order to escape a character we start it with a forward slash. In our example we can see that we are escaping the "." character before the "com" in our email.  This is because we need to escape the period since we know that it will be there. 

## Author

Nate Traugh

[GitHub](https://github.com/ntraugh)
