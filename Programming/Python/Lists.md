# Lists

### Lists use Brackets

Create a list:
```py
movie = ["Pacific Rim", "It", "The Hangover" ]
```

Accessing a list:
```py
print(movie[0]) #would return Pacfic Rim
print(movie[0:2]) #would return Pacific Rim and It
print(movie[0:]) #would return everything after Pacifc Rim
print(movie[:2]) #would return everything before The Hangover
print(movie[-1]) #would return the Hangover
```

Functions:
```py
len(movie) #would return the amont of objects in the list
movie.append("Jaws") #would add Jaws to the END of the list
movie.pop() #would remove the LAST item
movie.pop(0) #would remove the FIRST item
```