REGEX-TUTORIAL
A regular expression or regex is a pattern describing a certain amount of text.

Summary
A regular expression or also known as regex, is a sequence of hyrogliphoc-characters such as numbers, letters, percent-sign, arrows, dashes, ect., that defines a specific search pattern. Regex are extremely useful in finding and extracting data from any text by performing a specific search pattern using the hyrogliphio-characters.

Table of Contents
Anchors
Quantifiers
OR Operator
Character Classes
Flags
Grouping and Capturing
Bracket Expressions
Greedy and Lazy Match
Boundaries
Back-references
Look-ahead and Look-behind

Regex Components are commonly found in various programming languages, however, the implementation of the characters may differ.

Anchor components specifies a location within a particular string to search, they match postiions before, after or between characters. For example: * ^A = match at the beginning of a line.  * A$ = match at the end of a line.

Quantifiers ( * + ? {} ) allow for the specification of how many instances of a character, character-class or group must be present in the input for a match to be found. 
For an example: abc{2,5} matches a string that has ab followed by the numbers 2 up to 5 c

OR Operator (|) is used to match characters or expression of either the left or right of the operator. For an example (G|g) will match either G or g from the input string.

Character Classes are also known as character-sets are one of the most common used features of regex, they allow you to direct the regex engine to match only one out of several characters. Simply place the characters between square [ ] brackets. For an example, if you would want to match a letter 'k' and letter 'p' do the following [kp].

Flags are optional parameters to a regex that modifies its behavior of searching. A flag changes the default searching behaviour of a regular expression. A flag is denoted using a single lowercase alphagetic character.

Grouping and Capturing groups area a way to treat multiple characters as a single unit, they are created by placing the characters to be grouped inside a set of parentheses.

Bracket Expressions can be used to match a single character or collating element.

Greedy quantifiers match the longest possible string and Lazy Match quantifiers match the shortetst possible string. (* + {}) are greedy operator, so they expand the match as far as they can through the provided text.

Boundaries have various functions or uses, lets take a look at the different boundary-constructs.
* ^ The beginning of a line
* $ The end of a line
* \b A word boundary
* \B A non-word-boundary
* \A The beginning of the input
* \G The end of the previous match
* \Z The end of the input but for the final terminator, if any
* \z The end of the input

Back-references are captured-matched-input-strings saved in memory for later recall. The back-references are specified in the regular expression as a backslash ( \ ) followed by a digit in which indicates the number of the group to be recalled, for the example: (\r\r) defines one capturing group matching two-digits in a row, which can be recalled later in the expression via the backreference \1.

Look-ahead and Look-behind are also known as lookarounds that are considered as assertions in which don't deploy match-characters, they only indicate if there was a match or no-match.  

REGEX-DEMONSTRATION WITH THE EMAIL-MATCHING: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Author
Andres Abreu: https://github.com/andres-abreu