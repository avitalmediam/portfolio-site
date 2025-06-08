
###### Getting Started 

When pandoc is ==invoked without specifying any input files==, it operates as a “***filter***,” taking input from the terminal and sending its output back to the terminal. You can use this feature to play around with pandoc. ([source](https://pandoc.org/getting-started.html))

By default, input is ==interpreted as pandoc markdown== , and ==output is HTML==. But we can change that. Let’s try converting _from_ HTML _to_ markdown:

To convert it to HTML, use this command:

```
pandoc test1.md -f markdown -t html -s -o test1.html
```

The filename `test1.md`
 tells pandoc which file to convert. The ==” file, with a header and footer, not just a fragment. And the ==
`-o test1.html` says to put the output in the file `test1.html`.

# User Guide



Source: [Manual](https://pandoc.org/MANUAL.html)


# EPUB

Source: [Manual](https://pandoc.org/MANUAL.html#epubs)

EPUB metadata may be specified using the [`--epub-metadata`](https://pandoc.org/MANUAL.html#option--epub-metadata) option, but if the source document is Markdown, it is better to use a [YAML metadata block](https://pandoc.org/MANUAL.html#extension-yaml_metadata_block). Here is an example of a YAML metadata block with EPUB metadata:

```
---
title:
- type: main
  text: My Book
- type: subtitle
  text: An investigation of metadata
creator:
- role: author
  text: John Smith
- role: editor
  text: Sarah Jones
identifier:
- scheme: DOI
  text: doi:10.234234.234/33
publisher:  My Press
rights: © 2007 John Smith, CC BY-NC
ibooks:
  version: 1.3.4
...
```
