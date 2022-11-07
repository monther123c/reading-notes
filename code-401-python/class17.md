# Automation
---
### Regular expressions:
Are a powerful language for matching text patterns. The Python "re" module provides regular expression support.

- The re.search() :
method takes a regular expression pattern and a string and searches for that pattern within the string. If the search is successful, search() returns a match object or None otherwise.
Therefore, the search is usually immediately followed by an if-statement to test if the search succeeded,for example: search for the pattern 'word:' followed by a 3 letter word
---
- The code match = re.search(pat, str) stores the search result in a variable named match. Then the if-statement tests the match -- if true the search succeeded and match.group() is the matching text (e.g. 'word:cat'). Otherwise if the match is false (None to be more specific), then the search did not succeed, and there is no matching text.

- The 'r' at the start of the pattern string designates a python "raw" string which passes through backslashes without change which is very handy for regular expressions.

---
### Basic Patterns
The power of regular expressions is that they can specify patterns, not just fixed characters. Here are the most basic patterns which match single chars:

- a, X, 9, < -- ordinary characters just match themselves exactly. The meta-characters which do not match themselves because they have special meanings are: . ^ $ * + ? { [ ] \ | ( )

-  . (a period): matches any single character except newline '\n'
- \w: (lowercase w) matches a "word" character: a letter or digit or underscore [a-zA-Z0-9\_]. Note that although "word" is the mnemonic for this, it only matches single word char, not a whole word. \W (upper case W) matches any non-word character.
- \b: boundary between word and non-word
- \s: (lowercase s) matches a single whitespace character (space), newline, return, tab, form [ \n\r\t\f]. \S (upper case S) matches any non-whitespace character.
- \t, \n, \r: tab, newline, return
- \d: decimal digit [0-9] (some older regex utilities do not support but \d but they all support \w and \s)
- ^ = start, $ = end: match the start or end of the string
- \: inhibit the "specialness" of a character. So, for example, use \. to match a period or \\ to match a slash. If you are unsure if a character has special meaning, such as @, you can put a slash in front of it, \@, to make sure it is treated just as a character.
---
### Repetition
Things get more interesting when you use + and * to specify repetition in the pattern

- +: 1 or more occurrences of the pattern to its left, e.g. 'i+' = one or more i's
- *: 0 or more occurrences of the pattern to its left
- ?: match 0 or 1 occurrences of the pattern to its left

#### Leftmost & Largest
- First the search finds the leftmost match for the pattern, and second it tries to use up as much of the string as possible: i.e. + and * go as far as possible (the + and * are said to be "greedy")