# Brackets

## Context

Brackets !
They haunt you, even in your sleep !
Do they match ?
You don't know !
But you should...

## Summary

Your program must be able to return [EXIT_SUCCESS](http://www.cplusplus.com/reference/cstdlib/EXIT_SUCCESS/) if the string passed as parameter is a valid sequence of brackets, or [EXIT_FAILURE](http://www.cplusplus.com/reference/cstdlib/EXIT_FAILURE/) otherwise.

List of brackets:
- { .. }
- ( .. )
- [ .. ]

A valid sequence of brackets is defined as an open bracket, followed by a closing bracket. There can be N sequence of brackets between and after the opening and the closing bracket.

There can be [ASCII whitespace characters](http://www.cplusplus.com/reference/cctype/isspace/) between the brackets. They do not invalidate the sequence.

## Example

```
$ ./seq "[]"
$ echo $?
0

$ ./seq "[{ () }]"
$ echo $?
0

$ ./seq "[{}]([]){}{[]}"
$ echo $?
0

$ ./seq "["
$ echo $?
1

$ ./seq "[(]"
$ echo $?
1

$ ./seq "([()]("
$ echo $?
1
```

## FAQ

Q. What is that `echo $0` ?

A. [Yes.](https://www.gnu.org/software/bash/manual/html_node/Special-Parameters.html)
