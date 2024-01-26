Values will change because the compiler will guess at what `type` the outcome of the code will be. This can be changed with explicity.

### Implicit 
(Compilier guesses)
```c
double testScore = 95.7;
int displayScore = 0;  

displayScore = testScore;
```


### Explicit 
(Programmer told compiler what type)
```c
double testScore = 95.7;
int displayScore = 0;  

displayScore = (int)testScore;
```

### More Info

Sometimes it’s useful, or even necessary, to change the value type of a variable and use it for other purposes. For instance, if you had a `double` with a percent score on a test, say 0.95, you would most likely want to display 95% to the user instead. Notice, we are not changing the type of the variable, nor the value stored in the source variable. What we are doing is displaying the changed variable as a new type or storing it in a different variable that might be a different type.

So you could not do this:
```c
int a;
double b = 3.0;

a = b;
```

There are two types of conversions, implicit and explicit. When you set one variable to be the same as another, such as `a = b` above, but their types do not match, the compiler will try to convert them. However, this can be dangerous as you might not know what values will be in the variable at runtime, and it might not be implicitly convertible to another type. Our example above was implicit, the compiler in this case will make a best guess.

The other way to convert a variable from another type is explicitly. You can do this by simply telling the compiler what type you want to set it to. So in our example above we could change the line `a = b` to `a = (int)b`. That way if `b` was something other than 3.0, such as 3.2, we are telling the compiler to make it work, so it would set it to 3.

A more interesting casting option is converting a `char` to a number type, or the other way around. Just like before, you have to be careful how you set this up. In the back-end, a `char` doesn’t store `'a'`, it stores the value representing that: 97 for lowercase and 65 for uppercase.

```c
int targetInt;
char sourceChar = 'a';

targetInt = (int)sourceChar;
```

Now `targetInt` equals 97.

When you cast an `int` to a `char`, you get the opposite process and the `char` is set to the value at the `int` value. So if you did:

```c
int sourceInt = 65;
char targetChar;

targetChar = (char)sourceInt;
```

`targetChar` now equals `'A'`.


