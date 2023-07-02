# Regex Tutorial: Matching an Email

Matching an Email 

Regex Pattern for Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 

Your Challenge this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. You'll use the template provided in the starter code to create your tutorial.

## Summary

A regex, or a regular expression is a sequence of characters that deine a specific search patern. Each component of the regex has a uniqiue responsibility. The regex I wil be describing is the email. An example of the regex pattern to match an email is below. 

Regex Pattern for Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 

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

As aforementioned, this section will breakdown the Matching an Email regex pattern, and explain each of the componenets included in it. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors

The characters ^ and $ are anchor characters. The ^ anchor identifies a string that will begin a line of subsequent characters. Note, this is a case senstitve regex! So whereas a string match might be ^A, where the strings "A" or "A person" match, but the lowercase alternative if "a" and "a person" would not. 

### Quantifiers

As a reminder of regex pattern is as follows: Regex Pattern for Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 

Quantifiers set the limits of the string that the regex matches. They will frequently include the minumum and maximum number of characters that the regex is looking for. Quantifiers will match as many occurances of a particular pattern as possible. Meaning , they include:
* -Matches the pattern zero or more time
+ -Matches the pattern one of more times
? -Matches the pattern zero or one time
{} -Provides three different ways to set limites for a match:  { n } -Matches the pattern exactly n number of times, { n, } -Matches the pattern at least n number of times, and { n, x } -Matches the pattern a minimum of n times to a maximum of x times. 

The ? symbol placed after the brackets{} mean that it will match with a little occurances as possible. In our "Matching an Email" regex, the quantifier is {2,6}. Meaning, the preceding string pattern is a minumum of 2 times and the maxiumum of 6, with letter set of [a-z\]. 

### Grouping Constructs

Grouping Constucts break up sections. The first group in our expression is ([a-z0-9_\.-]+), which captures the users email username,  the second group is ([\da-z\.-]+) which captures the company @ (ex: gmail, yahoo), and the last group is ([a-z\.]{2,6}), which captures the .com. 

### Bracket Expressions

A bracket expression or a positive character group is nything that lives inside a set of square brackets [] indiciates a range of characters that will be matched. For example, [xyz] will be a string that will include the letters x, y, and z regardless of the length of the actual string. Example that would match would be: "xxx", "yyy", "zzz", "zyx", and "xypzyxyzr". 

### Character Classes
 
Character Class in a regex are used to match characters from a specific set or range. In our example \d matches any Arabic numeral digit, which is equal to the bracket expression [0-9].

### The OR Operator

An OR Operator (|) is used to match either the expression before or after it. For exmaple, the expression [xyz] could be written as (x|y|z). In our Matching an Email regex pattern, there is no use of the OR Operator.

### Flags

Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex. All together, there are six flags that can be used either sepateely, or together and in any order. In our Matching an Email regex pattern, there is no use of Flags.

### Character Escapes

The backlash (\) in a regex escapes a character that would orignially be treated as literally. For exmaple, adding a backslash before the open curly brace (\{) means that the regex needs to look for the open curly brace first. 

## Author

This tutorial is explained by Rachel McAllister. To find more information from Rachel McAllister, please visit [here] (https://github.com/rachelmcallister1)

