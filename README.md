# Learn Regex
Examples based regex learning

# Cheatsheet
| Symbol | Meaning |
| --- | --- |
| . | Any character except new line |
| \w | Word |
| \W | Not Word |
| \d | Digit |
| \D | Not Digit |
| \s | Whitespace |
| \S | Not Whitespace |
| [abc] | Any of a,b,c |
| [^abc] | Not any of a,b,c |
| [a-z] | Character from a to z |
| ^abc | Start of the string |
| abc$ | End of the string |
| \b | Start of the string |


# Character Handling
# Basic match
Match exact characters.

```
`name` => My `name` is Imran.
`apple` => I have an `apple` and a banana. My friend also has an `apple`.
```

## [abc] character set
Match any character in the set.

`[tT]he` => `The` man and `the` woman.

