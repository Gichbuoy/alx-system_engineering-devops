## Regular Expressions
- Regular expressions, often referred to as regex or regexp, are sequences of characters used to define search patterns in text. They are powerful tools for pattern matching and text manipulation, widely used in programming languages, text editors, and command-line tools.

- Regular expressions consist of a combination of literal characters and metacharacters, which have special meanings. Here are some commonly used metacharacters:

* . (dot): Matches any single character except a newline.
* * (asterisk): Matches zero or more occurrences of the preceding character or group.
* + (plus): Matches one or more occurrences of the preceding character or group.
* ? (question mark): Matches zero or one occurrence of the preceding character or group.
* [] (square brackets): Defines a character class, matching any single character within the brackets.
* [^] (caret within square brackets): Defines a negated character class, matching any character not within the brackets.
* | (pipe): Acts as a logical OR, matching either the expression before or after the pipe.
* () (parentheses): Groups characters or expressions together.
Here are a few examples of how regular expressions can be used:

### Matching a specific pattern:

* cat matches the word "cat" exactly.
* c.t matches any three-character string starting with 'c' and ending with 't', with any character in the middle.

### Matching characters within a range:

* [a-z] matches any lowercase letter.
* [0-9] matches any digit.


### Quantifiers:

* a* matches zero or more occurrences of the letter 'a'.
* a+ matches one or more occurrences of the letter 'a'.
* a? matches zero or one occurrence of the letter 'a'.


### Grouping and capturing:

* (ab)+ matches one or more occurrences of the string "ab".
* (foo|bar) matches either "foo" or "bar".
