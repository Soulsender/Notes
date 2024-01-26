#### Regex Characters
- `^` starts regex
- `$` ends regex
- `[]` contains (`[aeious]`, `0-9`)
- `[^]` is not
- `.` any character
- `.*` wildcard character
- `{}` of the proceeding matches (`{3}`)
- `()` multiple regex (seperated and ORed with `|`)
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
```

