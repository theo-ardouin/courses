# Morse

## Context

You are in 1845.
You own a mail agency company.
You have a computer that, oddly, can only send messages in morse.
Your computer is not anachronic in any way.
This is fine.
You must be able to send messages using the said computer.
That is it.

## Description

This program allows you to read from [standard input](https://en.wikipedia.org/wiki/Standard_streams) a [ASCII](https://en.wikipedia.org/wiki/ASCII) text and translate it into [morse code](https://en.wikipedia.org/wiki/Morse_code).
You must display the morse code on the [standard output](https://en.wikipedia.org/wiki/Standard_streams).

The program stops only when the user hits ctrl-C or ctrl-D.

If a character is not recognized (non-translatable into morse for instance), you must display an error message on the [standard error output](https://en.wikipedia.org/wiki/Standard_streams).

## Example

```
$ echo hello | ./morse
.... . .-.. .-.. ---

$ ./morse
> Hello, I am a text !
.... . .-.. .-.. --- --··--     ..     .- --     .-     - . -..- -     -·-·--
> twat
- .-- .- -
^C

$ ./morsii < file_that_contains_hello_world
.... . .-.. .-.. ---     .-- --- .-. .-.. -..
```
