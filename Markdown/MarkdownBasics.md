# Markdown Cheat Sheet
The flowinging cheat sheet is a summary of James Quick's tutorial. Go give him a view: 

<https://www.youtube.com/watch?v=pTCROLZLhDM>

If using VSCode can press `ctrl+shift+v` or `command+v` to live preview Markdown files.
Visual Studio Code uses the [CommonMark](http://commonmark.org/) Markdown specification.

---

## Headers
Headers are defined using the '#' symbol:

    # H1 Header 
    ## H2 Header
    ### H3 Header
    #### H4 Header
   

# H1 Header 
## H2 Header
### H3 Header
#### H4 Header

---

## Quotes


Quotes are defined using the  '>' symbol:

    > This is an example quote

> This is an example

Quotes can be added on top of other formatting. They are useful for TODO items:

    > **TODO** Fix bug

> **TODO** Fix bug

---

## Emphasis

Emphasis is added with either asterisks and underscores. Mix them together to create **bold** and _italicized_ text:

    *italicized text*
    **bold text**

    _italicized text_
    __bold text__

    _**bold and italicized text**_
    
*italicized text*
**bold text**

_italicized text_
__bold text__

_**bold and italicized text**_

---

## Horizontal Separators
Horizontal separators can be created with hypens, asterisks, or underscores:

    ---
    ***
    ___

---
***
___

## Lists

Create unordered lists using a plus, dash, or asterisk:

    - item a
    - item b
    - item c

    * item 1
      * item 1.1
        * item 1.1.1

    + apples
    + oranges


- item a
- item b
- item c

* item 1
  * item 1.1
    * item 1.1.1

+ apples
+ oranges

Create ordered lists using a number prefix. However, the format may change depending on the viewer:

    1. item 1
    2. item 2
       1. dsfdsfsdf
    3. item 3 


1. item 1
2. item 2
   1. dsfdsfsdf
3. item 3 

---

## External and Internal Links

Create a link by surrounding it with angle brackets:

    <http://www.github.com> 

<http://www.github.com> 

Links also be named:

    [Link to github](http://www.github.com)

[Link to github](http://www.github.com)

Reusable links can be made for code reusage:

        [1]: http://github.com/
        [Link to github][1]

[1]: http://github.com/
[Link to github][1]

Links can be created for locations in your Markdown page:

    [Links](#external-and-internal-links)

    [Sections](#sections)

[Links](#external-and-internal-links)

[Images](#sections)

---

## Images

Links to images can also be defined:


    Example

    ![Michaelangelo](https://i.kym-cdn.com/photos/images/original/000/377/873/c73.jpg) 

![Michaelangelo](https://i.kym-cdn.com/photos/images/original/000/377/873/c73.jpg) 

Image links can also be optimized for code reusage:

    [Patrick]: https://i.kym-cdn.com/entries/icons/original/000/025/580/Screen_Shot_2018-03-01_at_12.59.37_PM.png

    ![SavagePatrick][Patrick]

[Patrick]: https://i.kym-cdn.com/entries/icons/original/000/025/580/Screen_Shot_2018-03-01_at_12.59.37_PM.png

![SavagePatrick][Patrick] 

---

## Code

You can do inline code with backticks. They can be found on the tilda button: 

    Use the `run()` method to begin.

Use the `run()` method to begin.

Blocks of code can be defined using 3 backticks. Add the name of the programming language for proper syntax highlighting:

    ```Javascript
    var num = 0;
    var num2 = 0;
    ```

```Javascript
var num = 0;
var num2 = 0;
```

Here's another example using HTML:

    ```html 
    <div>
        <p>This is an html example</p>
    </div>
    ```

```html 
<div>
    <p>This is an html example</p>
</div>
```

---

## Tables
To create tables: 
- Header and row content are defined between pipes ( | )
- Rows are separated with at least 3 dashes (---)

        | Header 1    | Header 2    | Header 3    |
        | ----------- | ----------- | ----------- |
        | Row 1 Col 1 | Row 1 Col 2 | Row 1 Col 3 | 

| Header 1    | Header 2    | Header 3    |
| ----------- | ----------- | ----------- |
| Row 1 Col 1 | Row 1 Col 2 | Row 1 Col 3 | 


Avoid poor formatting because these can become hard to read:

    | Header 1 | Header 2 |
    | ----| ---|
    |Loooooooooooooong item 1 | looooooooooong item 2 | 

| Header 1 | Header 2 |
| ----| ---|
|Loooooooooooooong item 1 | looooooooooong item 2 | 

You can also define alignment for each row using colons:

    | Header | Header 1 | Header 2  |
    | ------ | :------: | --------: |
    | Aligned Left | Aligned Center | Aligned Right | 

| Header | Header 1 | Header 2  |
| ------ | :------: | --------: |
| Aligned Left | Aligned Center | Aligned Right | 
---

## Custom HTML

Since Markdown gets automatically converted to HTML, you can add raw HTML directly to your Markdown:

    <h2>Header In HTML Syntax</h2>

<h2>Header In HTML Syntax</h2>

However, Markdown syntax is almost always easier.

---

## Custom CSS

You can also add custom CSS to your Markdown to add additional styling to your document. For example, we could turn all heading 3 text red. However, this only works with compatible previews:

    <style>
    h5 {
        color: red
    }
    </style>

    ##### Header 5 text

<style>
    h5 {
        color: red
    }
</style>

##### Header 5 text

---

## Additional Resources
- [Markdown Cheat Sheet - Adam P on Github](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images)
- [Daring Fireball Markdown Syntax](https://daringfireball.net/projects/markdown/syntax)
- [Markdown in Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown)