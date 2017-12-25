# Bitmap

## Context

Ever wondered how some data would look like as image?
Probably not, because that is _really_ stupid...

Why am I still writing those?
Is my life slowly becoming a joke of some sort?
...

Nevermind! Sweet, sweet bmp is our topic today!

## Summary

The goal of the program is to be able to make a [BMP file](https://en.wikipedia.org/wiki/BMP_file_format) from scratch by reading [standard input](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)) to populate the said file.
You must pass as parameter the width of the image as the first argument.

You must stop your program (and flush the bmp file) whenever the user hits [Ctrl-C](https://en.wikipedia.org/wiki/Signal_(IPC)#Handling_signals) or when you stops reading data from the [standard input](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_(stdin)).

You must populate the file as the following: Read the 3 bytes to create a corresponding color (red, green, blue) and write them into the bmp file. Repeat the process.

You must be able to handle every size of file (within the limitation of your system), i.e, you must _not_ create a growing buffer of data.
Instead, use a fixed buffer and flush into the bmp file as soon as the buffer is full.

## Example

```
$ cat /dev/random | ./mtob 100
^C

$ cat ./some_random_file | ./mtob 20 hello.bmp
```
