- **wildcard mark bit 0** - match corresponding bit value in address
- **wildcard mask bit 1** - deny corresponding bit value in address
### How to find mask
```sh
# Example from .8 to .31
# convert to binary
8  = 00001000
32 = 00001111

# get differences
00001{111}

# replace with 1s
00000111

# convert back to decimal
7 = 00000111

# 0.0.0.7 is the wildcard mask
```