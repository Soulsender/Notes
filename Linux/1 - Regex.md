#### Regex Characters
- `^` starts regex
- `$` ends regex
- `[]` contains (`[aeious]`, `0-9`)
- `[^]` is not
- `.` any character
- `.*` wildcard character
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
```

