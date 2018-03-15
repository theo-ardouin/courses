# Bitmap

## Prerequisite

- Language: C
- Don't use external libraries
- [What is the bmp format?](https://en.wikipedia.org/wiki/BMP_file_format)

## Context

Our marketing guy just sold a software to a client that wants to know what's the color of the memory on his computer...

...

The hell?! Why did we even hired that guy?

Well, apparently, he does a very good coffee... Alright then.

## Summary

The goal of the program is to be able to make a [bmp file](https://en.wikipedia.org/wiki/BMP_file_format) from scratch by reading [standard input](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)) to populate the said file.
You must pass as parameter the width of the image as the first argument.

You must stop your program (and flush the bmp file) whenever the user hits [Ctrl-C](https://en.wikipedia.org/wiki/Signal_(IPC)#Handling_signals) or when you stops reading data from the [standard input](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)), or when the image is complete.

You must populate the file as the following: Read the 3 bytes to create a corresponding color (red, green, blue) and write them into the bmp file. Repeat the process.

You must be able to handle every size of file (within the limitation of your system), i.e, you must _not_ create a growing buffer of data.
Instead, use a fixed buffer and flush into the bmp file as soon as the buffer is full.

## Example

```
$ cat /dev/random | ./dtob 100
^C

$ cat ./some_random_file | ./dtob 20 hello.bmp
```
