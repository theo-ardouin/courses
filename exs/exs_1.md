# alphabet
Write a C function that displays the alphabet followed by a [newline](https://en.wikipedia.org/wiki/Newline), considering a flag that toggle [lower or upper case](https://en.wikipedia.org/wiki/Letter_case)

### Prototype
`void alphabet(int flag)`

### Example:
```
> alphabet(0);
< abcdefghijklmnopqrstuvwxyz

> alphabet(1);
< ABCDEFGHIJKLMNOPQRSTUVWXYZ

> alphabet(42);
< ABCDEFGHIJKLMNOPQRSTUVWXYZ
```

### Functions
* `int putchar(int)`


# int_to_bin
Write a C function that displays a [binary representation](https://en.wikipedia.org/wiki/Binary_number) of a number followed by a [newline](https://en.wikipedia.org/wiki/Newline)

### Prototype
`void int_to_bin(int number)`

### Example:
```
> int_to_bin(42);
< 101010

> int_to_bin(-42);
< -101010

> int_to_bin(1);
< 1
```

### Functions
* `int putchar(int)`

### Limitations
* Arrays _DO NOT_ exists, too bad :)

### Hints
* [Recursive](https://en.wikipedia.org/wiki/Recursion_(computer_science))
