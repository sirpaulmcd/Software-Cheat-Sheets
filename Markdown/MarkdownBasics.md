# Markdown Cheat Sheet
The flowinging cheat sheet is a summary of James Quick's tutorial. Go give him a view: 

<https://www.youtube.com/watch?v=pTCROLZLhDM>

If using VSCode can press `ctrl+shift+v` or `command+v` to live preview markdown files.
Visual Studio Code uses the [CommonMark](http://commonmark.org/) Markdown specification.

---

## Headers
Headers are defined by the '#'symbol.  One '#' for H1, two for H2, etc.

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


Quotes are defined by the  '>' symbol 

    > This is an example quote


> This is an example

Quotes can be added on top of other formatting. They are useful for TODO items

    > **TODO** Fix bug

> **TODO** Fix bug

---

## Emphasis

Add emphasis with either asterisks and underscores. Whichever you prefer. Mix them together to create **bold** and _italicized_ text.

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

## Horizontal Rule Separators
A horizontal rule gives a visible line break.  You can create one by putting three or more hypens, asterisks, or underscores (-, *, _).

    ---
    ***
    ___

---
***
___



## Lists

Create unordered lists using '-', '*', or '+'. Whichever you prefer

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

Create ordered lists using a number prefix. Unfortunately, sublist functionality is limited (have to start back at 1). 

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

Create a link by surrounding it with angle brackets. Can also name the link.

    <http://www.github.com> 

    [Link to github](http://www.github.com)

<http://www.github.com> 

[Link to github](http://www.github.com)

Create a reusable link (good practice)

        [1]: http://github.com/
        [Link to github][1]

[1]: http://github.com/
[Link to github][1]

Create a link to a location in your markdown page. Note that names must follow css convention. 

(I.e. External and Internal Links -> external-and-internal-links)

    [Links](#external-and-internal-links)
    [Sections](#sections)

[Links](#external-and-internal-links)

[Images](#sections)

---

## Images

Defining an image is similar to defining a link, except you prefix it with '!'


    Example

    ![Michaelangelo](https://i.kym-cdn.com/photos/images/original/000/377/873/c73.jpg) 

![Michaelangelo](https://i.kym-cdn.com/photos/images/original/000/377/873/c73.jpg) 

Images links can also be reused

    [Patrick]: https://i.kym-cdn.com/entries/icons/original/000/025/580/Screen_Shot_2018-03-01_at_12.59.37_PM.png

    ![SavagePatrick][Patrick]

[Patrick]: https://i.kym-cdn.com/entries/icons/original/000/025/580/Screen_Shot_2018-03-01_at_12.59.37_PM.png

![SavagePatrick][Patrick] 

---

## Code

You can do inline code with backticks. They can be found on the tilda button. 

    Use the `run()` method to begin.

Use the `run()` method to begin.

You can do blocks of code by surroung it with 3 backticks. You can also define the language for proper syntax highlighting.

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
Creating tables
- Header and row content defined between pipes (|)
- Rows are separated with a row of dashes (---). At least 3 are reqired. 

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

You can also define alignment for each row using colons

    | Header | Header 1 | Header 2  |
    | ------ | :------: | --------: |
    | Aligned Left | Aligned Center | Aligned Right | 

| Header | Header 1 | Header 2  |
| ------ | :------: | --------: |
| Aligned Left | Aligned Center | Aligned Right | 
---

## Custom HTML

Since MarkDown gets automatically converted to HTML, you can add raw HTML directly to your MarkDown.

    <h2>Header In HTML Syntax</h2>

<h2>Header In HTML Syntax</h2>

However, markdown syntax is almost always easier.

---

## Custom CSS

You can also add custom CSS to your MarkDown to add additional styling to your document. You can also include CSS by including a style tag.

    ```html
    <style>
        body {
            color:red;
        }
    </style>
    ```


```html
    <style>
        body {
            color:red;
        }
    </style>
```

For example, we could turn all heading 3 text red:

    <style>
    h3 {
        color: red
    }
    </style>

    ### Header 3 text



<style>
    h3 {
        color: red
    }
</style>

### Header 3 text

---

## Additional Resources
- [Markdown Cheat Sheet - Adam P on Github](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images)
- [Daring Fireball Markdown Syntax](https://daringfireball.net/projects/markdown/syntax)
- [MarkDown in Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown)