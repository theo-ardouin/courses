# alphabet
Write a C function that takes an int flag that toggle [lower/upper case](https://en.wikipedia.org/wiki/Letter_case) and display on [stdout](https://en.wikipedia.org/wiki/C_file_input/output#Variables) the alphabet followed by a [newline](https://en.wikipedia.org/wiki/Newline)

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
Write a C function that takes an int and display its [binary representation](https://en.wikipedia.org/wiki/Binary_number) on [stdout](https://en.wikipedia.org/wiki/C_file_input/output#Variables) followed by a [newline](https://en.wikipedia.org/wiki/Newline)

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
