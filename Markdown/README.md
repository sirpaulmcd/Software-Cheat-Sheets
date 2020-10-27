# Markdown Cheat Sheet

Markdown is a text-to-HTML tool for web writers. It is a convient way to write notes that can be converted to HTML or PDF. You may recognize the `.md` format on your github repo `README.md` files.

If using VSCode can press `ctrl+shift+v` or `command+v` to live preview Markdown files.
Visual Studio Code uses the [CommonMark](http://commonmark.org/) Markdown specification.

## Sections
- [Headers](#headers)
- [Quotes](#quotes)
- [Emphasis](#emphasis)
- [Horizontal-Separators](#horizontal-separators)
- [Lists](#lists)
- [Links](#links)
- [Images](#images)
- [Videos](#videos)
- [Code](#code)
- [Tables](#tables)
- [Custom-HTML](#custom-html)
- [Custom-CSS](#custom-css)
- [Additional-Resources](#additional-resources)

---

## Headers
### Headers are defined using the '#' symbol:

    # H1 Header 
    ## H2 Header
    ### H3 Header
    #### H4 Header
    etc.

    Alternative H1 Header 
    ===

    Alternative H2 Header
    ---

# H1 Header 
## H2 Header
### H3 Header
#### H4 Header
etc.

Alternative H1 Header 
===

Alternative H2 Header
---

---

## Quotes

### Quotes are defined using the  '>' symbol:

    > Did somebody say pasta?

> Did somebody say pasta?

### Quotes can be added on top of other formatting. They are useful for TODO items:

    > **TODO** Eat pasta

> **TODO** Eat pasta

---

## Emphasis

### Words can be bolded, italicized, underlined, and striked:

    Bold using double **asterisks** or __underscores__

    Italicize using single *asterisks* or _underscores_

    Underline using HTML <ins>ins tags</ins>

    Strikethrough using double ~~tildes~~ 

    Do multiple using a <ins>~~_**combination**_~~</ins> of the above

Bold using double **asterisks** or __underscores__

Italicize using single *asterisks* or _underscores_

Underline using HTML <ins>ins tags</ins>

Strikethrough using double ~~tildes~~ 

Do multiple using a <ins>~~_**combination**_~~</ins> of the above

---

## Horizontal Separators
### Horizontal separators can be created with hypens, asterisks, or underscores:
    Hyphens:
    
    ---
    Asterisks:
    ***
    Underscores:
    ___

Hyphens:

---
Asterisks:
***
Underscores:
___

## Lists

### Create unordered lists using a plus, dash, or asterisk:

    - item a
    - item b
    - item c

    * list item 1
      * sublist item 1.1
        * sub-sublist item 1.1.1

    + apples
    + oranges


- item a
- item b
- item c

* list item 1
  * sublist item 1.1
    * sub-sublist item 1.1.1

+ apples
+ oranges

### Create ordered lists using a number prefix. Formats may vary with previewer:

    1. item 1
    2. item 2
       1. item 2.1
    3. item 3 


1. item 1
2. item 2
   1. item 2.1
3. item 3 

---

## Links

### External Links:

    Links without titles can be in the form of:
    - http://www.github.com 
    - <http://www.github.com> 
    - github.com (May not work in certain previews)

    [Titled link](http://www.github.com)

    [Titled link with hover description](http://www.github.com "Github Homepage")

    [1]: http://www.github.com
    [Referencable link for code reuse][1]

    [Link to a relative repository file](../blob/../Git/Git%20Commands.pdf)

Links without titles can be in the form of:
- http://www.github.com 
- <http://www.github.com> 
- github.com (May not work in certain previews)

[Titled link](http://www.github.com)

[Titled link with hover description](http://www.github.com "Github Homepage")

[1]: http://www.github.com
[Referencable link for code reuse][1]

[Link to a relative repository file](../blob/../Git/Git%20Commands.pdf)

### Internal Links:

    [Link to beginning of document](#markdown-cheat-sheet)

    [Link to additional resources](#additional-resources)

[Link to beginning of document](#markdown-cheat-sheet)

[Link to additional resources](#additional-resources)

---

## Images

### Unformatted images:

    In-line image link
    ![Github Logo](https://tinyurl.com/ydxejrh3) 

    Referenced image link
    [PatrickRef]: https://tinyurl.com/yafb79ct
    ![SavagePatrick][PatrickRef]

In-line image link:

![Inline](https://tinyurl.com/ydxejrh3) 

Referenced image link:

[PatrickReference]: https://tinyurl.com/yafb79ct
![SavagePatrick][PatrickReference]


### Formatted Images:
Use HTML syntax to format images. For example, resizing and centering:

    <p align="center">
        <img src="https://tinyurl.com/ydduzoo3" alt="michaelangelo" width="200" height="200" />
    </p>

<p align="center">
    <img src="https://tinyurl.com/ydduzoo3" alt="michaelangelo" width="200" height="200" />
</p>

---

## Videos

### Embedded YouTube videos snippet template:
Unfortnately, videos cannot be embedded into standard markdown. One workaround is to use the thumbnail image of the video as the link to the video.
This can be done easily by pasting the youtube video ID into the the following template:

    [![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

### For example:
If the video I want to link is `https://www.youtube.com/watch?v=lXMskKTw3Bc`, then the video ID is `lXMskKTw3Bc`. 
Therefore, after pasting the ID into the template, I have: 
        
    [![RickAstley](http://img.youtube.com/vi/lXMskKTw3Bc/0.jpg)](http://www.youtube.com/watch?v=lXMskKTw3Bc)

[![RickAstley](http://img.youtube.com/vi/lXMskKTw3Bc/0.jpg)](http://www.youtube.com/watch?v=lXMskKTw3Bc "Never Gonna Hit Those Notes")


## Code

### Indicate inline code with backticks found on the tilde key:

    Use the `run()` method to begin.

Use the `run()` method to begin.

### Indicate blocks of code using 3 backticks:

Add the name of the programming language for proper syntax highlighting.

    ```Javascript
    var num = 0;
    var num2 = 0;
    ```
    ```html 
    <div>
        <p>This is an html example</p>
    </div>
    ```
    ```
    def no_language_defined(a, b):
        return a-b
    ```

```Javascript
var num = 0;
var num2 = 0;
```
```html 
<div>
    <p>This is an html example</p>
</div>
```
```
def no_language_defined(a, b):
    return a-b
```
---

## Tables
### To create tables: 
- Header and row content are defined between pipes ( | )
  - Outer pipes are optional, alignment not necessary
- Rows are separated with at least 3 dashes (---)

```
| Header 1    | Header 2    | Header 3    |
| ----------- | ----------- | ----------- |
| Row 1 Col 1 | Row 1 Col 2 | Row 1 Col 3 | 
```

| Header 1    | Header 2    | Header 3    |
| ----------- | ----------- | ----------- |
| Row 1 Col 1 | Row 1 Col 2 | Row 1 Col 3 | 


### Align column text using colons:

    | Header   | Header 1 | Header 2 |
    | -------- | :------: | -------: |
    | Left     | Center   | Right    | 

| Header   | Header 1 | Header 2 |
| -------- | :------: | -------: |
| Left     | Center   | Right    | 

---

## Custom HTML

Markdown accepts HTML syntax:

    <h3>H3 Header In HTML Syntax</h3>

<h3>H3 Header In HTML Syntax</h3>

This is useful for features not built into Markdown such as image resizing and page customization. 

---

## Custom CSS

Markdown accepts CSS syntax:

    <style>
    h5 {
        color: red
    }
    </style>

    ##### Header 5 text

(May not work in certain previews)

<style>
    h5 {
        color: red
    }
</style>

##### Header 5 text

---

## Additional Resources

This cheat sheet was constructed using information from:
- [James Quick's Markdown Worksheet](https://github.com/jamesqquick/markdown-worksheet/blob/master/worksheet.md)
- [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

Official Documentation:
- [Daring Fireball Markdown Syntax](https://daringfireball.net/projects/markdown/syntax)
- [Markdown in Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown)

Recommended Markdown editors:
- [Typora](https://typora.io/)
- [Bear](https://bear.app/) - iOS only :(
