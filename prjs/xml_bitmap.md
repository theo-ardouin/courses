# Bitmap

## Prerequisite

- Language: C
- Don't use external libraries
- [What is the bmp format?](https://en.wikipedia.org/wiki/BMP_file_format)

## Context

//TODO

## Summary

The goal of the program is to be able to make a [bmp file](https://en.wikipedia.org/wiki/BMP_file_format) from scratch by reading a simple [XML](https://en.wikipedia.org/wiki/XML) configuration file to populate the said file.
You must pass as parameter the .bmp output file as first parameter, the second being the path of the configuration file.

The configuration file should look like the following:
```
<bitmap>
  <rectangle>
    <color>
      <r>0</r>
      <g>255</g>
      <b>0</b>
    </color>
    <x>0</x>
    <y>0</y>
    <height>10</height>
    <width>10</width>
  </rectangle>
</bitmap>
```
Don't forget to handle possible error cases!

## Example

```
$ ./xtob my_image.bmp my_config.xml
```
