# Basic Markdown Examples

Markdown is a simple text formatting language similar to HTML or LaTeX, but trading reduced functionality for simplicity and a short learning curve\.
Much like LaTeX a single carriage return does not start a new line in the output, unless you add two spaces to the end of the line or 
the new line starts with a control symbol\.

Markdown uses a set of reserved characters (control symbols) to provide formatting, if you need to use these characters in your text then you can escape 
them by putting a backslash \(\\\) in front of them\:
-  \\ backslash itself
-  \` backtick
-  \* asterisk
-  \_ underscore
-  \{ \} curly braces
-  \[  \] square brackets
-  \( \) parentheses
-  \# hash mark
-  \+ plus sign
-  \- minus sign (hyphen)
-  \. dot
-  \! exclamation mark

Some implementations of Markdown viewer will also render HTML tags, but others will not.

Markdown has gained most traction in producing documentation for open source projects, in partiular on GitHub where each 
project is automatically created with a readme\.md (\.md is the file extension for a Markdown file) in it's root for documenting 
the project and offering guidance to potential users and contributors.

The main advantages of Markdown over WYSIWYG word processors such as Word or Pages include\:
-  Being plain text Markdown documents can be edited on pretty much any platform including web based editors \(files 
in this project have been created direct on GitHub, on a Windows 10 PC, a Windows 11 PC, a MacBook and an iPad\)
-  Being plain text the files are likley to be accessible long after propietary formats used in WYSIWYG wordprocessors have faded into history
-  Files tend to be smaller than the equivalent WYSIWYG files
-  If for some reason you don't have access to a Markdown viewer, the text is readable ad formatting is mostly inferrable.
-  If part of a file gets corrupted the rest of the file is still readable
-  The format is extendable, for example Mermaid is an extention of Markdown that allows charts and images to be produced, so long as the viewers support the extention

Key disadvantages include\:
- Not as fully featured as most WYSIWYG workprocessors 
- A bit of learning curve to become competent, but less than say HTML or LaTeX
- Have to write your text with the control symbols then run the file through a viewer to see the effect, 
although plugins for common IDEs such as VS.Code and onoine editors often provide a preview pane
-  Can be a bit fussy about white\-space
-  May render slightly differently in different viewers, although it will still be comprehensible, 
  a heading 1 will still visibly higher level than a heading two but how that is achieved may differ
  and you cannot dictate the viewer renders elements \(e.g. the font used or the style of bullet in a list\)

## Headings

To make a line of text a heading just start the line with a \#, Markdown supports 5 levels of heading, 
level 1 uses a single \# and each \# you add up to \#\#\#\#\# takes it down one level

# Heading 1 - \#
## Heading 2 - \#\#
### Heading 3 - \###
#### Heading 4 - \####
##### Heading 5 - \#####

## Emphasis

###Bold

To make text bold, enclose it in a pair of astrisks, \*\*, or underscores, \_\_\.


**The quick brown fox jumps over the lazy dog.**
__The quick brown fox jumps over the lazy dog.__

###Italic

To make text italic, enclose it in a single asterisk, \*, or underscore, \_\.


*The quick brown fox jumps over the lazy dog.*
_The quick brown fox jumps over the lazy dog._



### Bold and Italic

You can combine both, \*\*\_ or \_\_\*, to get bold and italic text\.

**_The quick brown fox jumps over the lazy dog._**

## Tables

To crete a table start each row with a pipe-symbol, \|, then divide the columns with a pipe-symbol.

e.g. \| Col1 \| Col2 \| Col3 \|

To control the alignment of items in a table you can create the **second row** of the table with flags showing how that column should be displayed\:
-  Default Alignment \- \-
-  Left Alignment \- \:\-
-  Centre Alignment \- \:\-\:
-  Right Alignment \- \-\:

## Strike-Through

To ~~strke-through~~ text just put it between two pairs of the tilde (\~) symbol, e.g. \~\~strike-through\~\~


| Default | Left align | Center align | Right align |
| - | :- | :-: | -: |
| 9999999999 | 9999999999 | 9999999999 | 9999999999 |
| 999999999 | 999999999 | 999999999 | 999999999 |
| 99999999 | 99999999 | 99999999 | 99999999 |
| 9999999 | 9999999 | 9999999 | 9999999 |

## Block Quotes

To include text as a block quote \(e.g. a block of text from a document or communication\), start each line with a breather than symbol, />\.

e.g. \> This text is blockquoted  
\>\> This text if blockquoted two levels

> This text is blockquoted
>> This text if blockquoted two levels

## Lists

### Unordered List

An unordered \(bulleted\) list can be created by starting each line in the list with a hyphen, \-, if the list has multiple levels 
\(some list items break down into further detail) this can be achieved by indenting the detail items.  Depending on the Markdown 
viewer used the detail items may use a visually different bullet but it is not possoble to control what is used.

e.g. \- first item  
\- second item  
  \- detail of second item. 
  \- etc  
\- third item

- first item
- second item
  - detail of second item
  - etc
- third item

### Ordered List

An ordered \(numbered\) list can be created by starting each item with a digit, 0 to 9, followed by a full stop, \., or closing parenthesis.  
The 0 to 9 limit, giving a maximum of 10 items per ordered list, is as a result of problems with integer overflow errors in some Markdown viewers.

e.g.

1. First item
2. Second item
3. Third item

or

0) Item zero
1) Item one
2) Item two
3) Item 3

If you need more than 10 items in a list then consider looking at how to split the list into smaller chunks or combining items.  It is worth
bearing in mind that, from a User Experience \(often abbreviaed to UX\) perspective, long monolithic lists can be overwhelming.  Dividing the list into 
logically separate chunks, e.g. if the list is a process that someone must follow then perhaps breaking when they switch tool or submit a screen or form,
can make it easier to follow\.  Even lists such as scores in sportign or academic competitions can be most easily under stood if broken into top 10, 
next 10 and so on\.

## Code Highlighting

To include program code, also works for mathematical formulas (although Markdown doesn't have the abilituy to represent maths that LaTeX does),
enclose it between a backtick \(also called a backquote\), \`.

e.g. This is some \`code\`

This is some `code`




