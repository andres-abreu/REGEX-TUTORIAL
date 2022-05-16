# REGEX-TUTORIAL
A regular expression or regex is a string of text-patterns or text-hyrogliphocs that help match, locate and manage text. Regex is supported in all the scripting languages such as Perl, Python, PHP, JavaScript as well as general purpose programming languages such as Java and Word for searching texts.

## SUMMARY
A regular expression or also known as regex, is a sequence of hyrogliphoc-characters such as numbers, letters, percent-sign, arrows, dashes, ect., that defines a specific search pattern. Regex are extremely useful in finding and extracting data from any text by performing a specific search pattern using the hyrogliphio-characters and can be used to set input-parameters for users such as emails, passwords, ect. 

## TABLE OF CONTENTS
* Anchors
* Quantifiers
* OR Operator
* Character Classes
* Flags
* Grouping and Capturing
* Bracket Expressions
* Greedy and Lazy Match
* Boundaries
* Back-references
* Look-ahead and Look-behind

### Regex Components
Are commonly found in various programming languages, however, the implementation of the characters may differ. The following is an example with some of the regex components: 
~EXAMPLE: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchor components 
Specifies a location within a particular string to search, they match postiions before, after or between characters. For example: 
* ^A = match at the beginning of a line. 
* A$ = match at the end of a line.

### Quantifiers ( * + ? {} ) 
Allow for the specification of how many instances of a character, character-class or group must be present in the input for a match to be found. 
For an example: abc{2,5} matches a string that has ab followed by the numbers 2 up to 5 c

### OR Operator (|) 
Is used to match characters or expression of either the left or right of the operator. For an example (G|g) will match either G or g from the input string.

### Character Classes 
Are also known as character-sets are one of the most common used features of regex, they allow you to direct the regex engine to match only one out of several characters. Simply place the characters between square [ ] brackets. For an example, if you would want to match a letter 'k' and letter 'p' do the following [ kp ].

### Flags 
Are optional parameters to a regex that modifies its behavior of searching. A flag changes the default searching behaviour of a regular expression. A flag is denoted using a single lowercase alphagetic character.

### Grouping and Capturing groups 
Are a way to treat multiple characters as a single unit, they are created by placing the characters to be grouped inside a set of parentheses.

### Bracket Expressions 
Can be used to match either a matching list expression or a non-matching list expression such as collating-elements, collating-symbols, equivalence-classes, character-classes or range-expressions.

### Greedy quantifiers 
Match the longest possible string, for the example: (* + {}) are greedy operator, so they expand the match as far as they can through the provided text.
**Lazy quantifiers** are the opposite to the greedy quantifiers, they repeat a minimal number of times, for the example: +? matchies the preceding character or subexpression 1 or more times, however, as few as possible.

### Boundaries 
Have various functions or uses, lets take a look at the different boundary-constructs.
* ^ The beginning of a line
* $ The end of a line
* \b A word boundary
* \B A non-word-boundary
* \A The beginning of the input
* \G The end of the previous match
* \Z The end of the input but for the final terminator, if any
* \z The end of the input

### Back-references 
Are captured-matched-input-strings saved in memory for later recall. The back-references are specified in the regular expression as a backslash ( \ ) followed by a digit in which indicates the number of the group to be recalled, for the example: (\r\r) defines one capturing group matching two-digits in a row, which can be recalled later in the expression via the backreference \1.

### Look-ahead and Look-behind 
Are also known as lookarounds that are considered as assertions in which don't deploy match-characters, they only indicate if there was a match or not. 

### REGEX-BREAK-DOWN-EXPLANATION
**REGEX-EMAIL-EXAMPLE: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/**
**~1:** /^([a-z0-9_\.-]+)
* / begins with regex boundary
* ^ anchor asserts the position at the start of the string
* () parenthesis creates a group
* [] matches anything within the brackets
* a-z0-9 matches any lower-case-alphabet-letter from a to z & any numeric number from 0 to 9
* _\.- matches these characters
* + a quantifier that matches as many times as possible

**~2:** @ = matches the @ symbol

**~3:** ([\da-z\.-]+)
* () parenthesis creates a group
* [] matches anything within the brackets
* /d matches any mumeric digit
* a-z matches any lower-case-alphabet-letter from a to z
* \.- matches these characters
* + a quantifier that matches as many times as possible

**~4:** ([a-z\.]{2,6})$/
* () parenthesis creates a group
* [] matches anything within the brackets
* a-z matches any lower-case-alphabet-letter from a to z
* \. matches these characters
* {2,6} these greedy quantifiers matches the previous token 2 to 6 times as many times as possible
* $ this asserts the postion at the end of the string

### Author
Andres Abreu: https://github.com/andres-abreu