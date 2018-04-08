# split
Write a C function that splits a string into substrings using a list of separator. This function MUST NOT alter the original string.

### Prototype
`char** split(const char* str, const char* separators)`

### Example
```
> split("hello world!", " ");
< "hello", "world!"

> split("this-is_a string", " -_");
< "this", "is", "a", "string"
```

### Functions
* malloc()
* free()


# prettify
Write a C program that prettify a list of strings, read from [stdin](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)).
The program stops only when the user hits [Ctrl-C](https://en.wikipedia.org/wiki/Signal_(IPC)#Handling_signals) or [Ctrl-D](https://en.wikipedia.org/wiki/End-of-Transmission_character).
A string can be protected with double quotes. Backslashes must be considered as an [escape character](https://en.wikipedia.org/wiki/Escape_character).

All memory allocated MUST be deallocated !

### Example
```
$ ./prettify
> hello
> world
< hello world

> ./prettify
>   hello
>     world   
< hello world

> ./prettify
> It's   me,   
>    "  MARIO"     
> ^C
< It's me,   MARIO

> ./prettify
>   escape   me  \"   
> ^C
< escape me "
```

### Functions
* malloc() and alternatives
* free()
* signal()
* fgets()

### Hints
* [xargs](https://en.wikipedia.org/wiki/Xargs) is a binary with a close behaviour
* [Linked list](https://en.wikipedia.org/wiki/Linked_list)
* [Array](https://en.wikipedia.org/wiki/Array_data_structure)
