# substr
Write a C function that finds a substring without considering the [case](https://en.wikipedia.org/wiki/Letter_case) and returns the position of the first occurence, -1 otherwise.

### Prototype
`size_t substr(const char str[], const char substring[])`

### Example:
```
> substr("hello world", "world");
< 6

> substr("HELLO WORLD", "world");
< 6

> substr("HeLlO wOrLd", "WoRlD");
< 6

> substr("HeLlO wOrLd", "z");
< -1
```


# capitalize
Write a C function that displays and capitalize the first letter of every word followed by a [newline](https://en.wikipedia.org/wiki/Newline). The string must be trimmed

### Prototype
`void capitalize(const char str[])`

### Example:
```
> capitalize("hello");
< Hello

> capitalize("hello world");
< Hello World

> capitalize("  hello  \t  world  ");
< Hello World
```

### Functions
* `int putchar(int)`

### Hints
* Spaces characters are: ` \t\f\v\n\r`


# sort_this
Write a C function that sorts an array from a non-sorted array followed by a [newline](https://en.wikipedia.org/wiki/Newline)

### Prototype
`void sort_this(int array[], unsigned length)`

### Example:
```
> int array[] = { 0 };
> sort_this(array, 1);
< 0

> int array[] = { -1, 0 };
> sort_this(array, 2);
< -1, 0
```

### Functions
* `int putchar(int)`
