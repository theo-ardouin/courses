# Michel's Printf

## Prerequisite

- Language: C
- Forbidden functions: printf() and alike
- [What are variadic functions ?](https://en.wikipedia.org/wiki/Variadic_function)
- [What is ASCII ?](https://en.wikipedia.org/wiki/ASCII)

## Context

Your name is Michel.
You need to display strings, depending on the format, for an unknown number of variable.
However, as you don't find in the [_printf_](https://linux.die.net/man/3/printf) function a specifier to display a number with a 'michel' base, nor a binary base, you decide to make your own.

## Summary

Your C function should be much like the [_printf_](https://linux.die.net/man/3/printf) function.
It must handle the [followings specifiers](http://www.cplusplus.com/reference/cstdio/printf/):
- d
- u
- c
- s
- x
- X
- %

Moreover, as you are _Michel_, you will need _very_ specific specifiers for your own _michel_printf_. Those are described here:

| Specifier |	Output | Example |
|-----------|--------|---------|
| m | Unsigned michel integer, lowercase | iim |
| M | Unsigned michel integer, uppercase | IIM |
| b | Unsigned binary integer | 101010 |
| r | Reversed string | dlrow olleh |
| t | Trimmed string | hello world |
| K | Capitalize string | Hello World |

However, you don't really need to implement the _flags_, _width_ or _precision_ of the standard _printf_. Those are for suckers.


## Example

```
michel_printf("%s %d %u %b %x %X %m\n", "42", 42, 42, 42, 42, 42, 42);
(stdout) 42 42 42 101010 2a 2A iim
```

```
michel_printf("%s - %r - %t - %K\n", "hello world", "dlrow olleh", "\t hello world\t ", "hello world");
(stdout) hello world - hello world - hello world - Hello World
```
