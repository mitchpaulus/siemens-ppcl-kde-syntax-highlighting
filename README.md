# Siemens PPCL KDE Syntax Highlighting

This is a syntax highlighting definition file for the Siemens PPCL language.
It is an XML file in the KDE syntax highlighting schema.

[Pandoc](https://pandoc.org/) makes use of this format.

You can use this file to syntax highlight your markdown files like (without the `>` characters):

```
> ```ppcl
> 00100	IF("%A%SF_S" .EQ. OFF .OR. "%A%SF_C" .EQ. OFF) THEN SET(0,"%A%STOT")
> ```
```

and then compile using the Pandoc `--syntax-definition` option.

```sh
pandoc --syntax-definition ppcl.xml -o out.docx in.md
```

The documentation for the syntax highlighting file formatting is at: <https://docs.kde.org/stable5/en/kate/katepart/highlight.html>.
