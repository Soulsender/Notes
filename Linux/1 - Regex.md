#linux
#### Regex Characters
- `^` starts regex
- `$` ends regex
- `[]` contains (`[aeious]`, `0-9`)
- `[^]` is not
- `.` any character
- `.*` wildcard character
- `{}` of the proceeding matches (`{3}`)
- `()` multiple regex (separated and ORed with `|`)
- `?` last regex is optional
- `+` last character can be one or more
- `*` last character can be zero or more
- `{,}` consecutive digits
#### Grep Switches
- `-E` extended grep
- `-i` case insensitive
#### Examples
```bash
# starts with vowel
'^[aeiou]'

# ends with vowel
'[aeiou]$'

# contains two vowels in one word
'^[aeiou].*[aeiou]$'

# two vowels next to each other
'^[aeiou][aeiou]$'

# numbers in the range of 100000 - 999999
'^[1-9][0-9]{5}$'

# two regex ORed
'(^[89]....|[1-9]....$)'

# colour and color ("u" is optional)
'^colou?r$'
```

