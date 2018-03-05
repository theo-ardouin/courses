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

This program allows you to read from [standard input](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)) an [ASCII](https://en.wikipedia.org/wiki/ASCII) text and translate it into [morse code](https://en.wikipedia.org/wiki/Morse_code).
You must display the morse code on the [standard output](https://en.wikipedia.org/wiki/Standard_streams#Standard_output_(stdout)).

The program stops only when the user hits [Ctrl-C](https://en.wikipedia.org/wiki/Signal_(IPC)#Handling_signals) or [Ctrl-D](https://en.wikipedia.org/wiki/End-of-Transmission_character).

If a character is not recognized (non-translatable into morse for instance), you must display an error message on the [error output](https://en.wikipedia.org/wiki/Standard_streams#Standard_error_(stderr)).

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
