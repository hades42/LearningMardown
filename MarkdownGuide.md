#Mardown Guide
**Note**: This is my learning process from the book **Markdown Guide** by *Matt Cone*.
If by anychance there are someone see this and want to follow the steps I already did, I highly recommend you using a application where you can preview Markdown so you can know what's going on under the hood. I personally using **VSCode** and having a plug-in called **Markdown Preview Enhanced**. 
You can also watch this [video](https://www.youtube.com/watch?v=HUBNt18RFbo) for quick starting.

# About Heading
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
...

**Note**: So creating heading in Markdown is really similar to create heading in html. The number of signs we use should correspond to the heading level in html.
    *Example*:  
    # == \<h1>
    ## == \<h2>
    ... 

# Paragraphs
Using a blank line

to separate one or more lines of text.

# Line Break
To create a line break (\<br>), we need to end each line   
with two or more spaces and the press return.

*Example*:
This is the first line |space||space||return|  
The second line will immediately to down.

**Note**: But we can also use **\<br>** since Markdown also supports it if you find using space is annoying

# Bold Text
Adding two asterisks or underscores before and after a word or phrase. We can also using **\<strong>**{ *put the text here* }**\</strong>** for making bold text since Markdown also support it.

#Italic
Similar to bolding text put we only put **one asterisks** or underscore instead of two before and after a word or phrase. We can also using **\<em>**{ put your text here }**\<em>** for making italic text.

# Bold and Italic

Similar to those two above but we gonna use ***Three asterisks*** instead. <br>
We can using the combination of \<strong> and \<em> :   
**\<strong>** **\<em>** { put your text here } **\<strong>** **\<em>**

# Block Quote
To create a blockquote, we add a **>** in front of a paragraph.  
Or we can use html tag:  
 **\<blockquote>**{ *Your text going here* } **\</blockquote>**

> This is a blockquote
<blockquote> 
<p>This is also a blockquote but using html tag </p>
</blockquote>

# Block quote with multiple Paragraph
Just adding a **>** on the blank lines between the graph.

*Example*:
>This is the first line.  
>
>This is the second line.

# Neseted Blockquote
Adding **>>** in front of the paragraph

> This is the first line.
>
>> This is a nested paragraph.

# Blockquotes with any other elements
Making sure to have the sign **>** to define a blockquote first and then combine it with other elements.

> ##### This is for Testing blockquote combination
> * First item
> * Second item
> ***Pretty nice***

# Lists
### Ordered Lists
Adding line items with numbers followed by periods. The numbers dont have to be in numerical order, but the list should start with the number one.

1. First item.
2. Second item.
3. Third item.
4. Fourth item.

##### Nesting lists Items  
To nest line items on an ordered list, indent the items four spaces or **one tab**.

1. First item.
2. Second item.
    1. First of second item.
    2. Second of second item.
3. Third item. 

### Unordered Lists
To create unordered list, add dashes (**-**), asterisks (**\***) or plus sign (**+**) in front of the line

- First item
- Second item
- Third item
- Fourth item

##### Nesting lists Items  
- First item
- Second item
    - First of second item
    - Second of second item
- Third item

# Adding elements in Lists
Adding another elements in a list while preserving the continuity of the list, indent the element **four spaces** or **one tab**

- This is the first item
- This is the second item
    Oh I need to add something below the second item
- This is the third item

### Blockquotes

- This is the first item
- This is the second item
    >Oh I need to add something below the second item
- This is the third item


# Code Blocks
Code blocks are normally intended **four spaces** or **one tab**

    <html>
        <head>
            <p>Test</p> 
        </head> 
    </html>

Nowaday, people usually use **three backtichs (\`\`\`)** for openning and **three backticks (\`\`\`)** for closing the code block and define the programming language for it

*Example*: 
\`\`\`c++ <br> {your code will go here} \`\`\`

```c++
int main(){
    cout << "hello world" << endl; 
}
```

# Horizontal rule
To create horizontal rule, use three or more asterisks (***), dashes(---) or underscores(___) on a line by themselvesa.

***

___

---

**Note**: For compatibility, put blank lines before and after horizontal rules

*Example*:
Try to put a blank line before...

---

... and after horizontal rule.


# Links
To create a link, enclose the link text in brackets (eg, [Youtube]) and then follow it immediately with the URL in parenthesis(eg., (https://youtube.com)).  
We can also use **\<a>** **\<a>** like the way we usually do in HTML to attach a link on the website.

[YOUTUBE](https://www.youtube.com/watch?v=lTRiuFIWV54&t=300s)

## Adding title
We can add a title for a link. This will apear as a tooltip when the user hovers over the links. To add a title, enlose it in parentheses after the URL

[YOUTUBE](https://www.youtube.com/watch?v=lTRiuFIWV54&t=300s "Lofi music")

## URLs and Email Addresses
To quickly turn a URL or email address into a link, enclose it in angle bracket
<Fake_Email@gmail.com>
  
## Formatting links
To **emphasize** links, add asterisks before and after the brakets and parentheses.

I love **[LOFI](https://www.youtube.com/watch?v=lTRiuFIWV54&t=300s "Lofi music")**


# Reference-style Links
Reference-style links are constructed in two parts: The part you keep inline with your text and the part you store somewhere else in thefile to keep the text easy to read.

### Formatting the first part
The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of bracket displays a label used to point to the link you're storing elsewhere in your document.

- [Lofi-music][1]
- [Lofi-music][2]

### Formatting the second part
1. The label, in brackets, followed immediately by a colon and at least one space (eg, [label]: ).
2. The url for the link, which we can optionally enlose in angle bracket.
3. The optional title for the link, which we can enlose in double quotes, single quotes, or parenthesis

- \[1]: <https://www.youtube.com/watch?v=lTRiuFIWV54&t=300sa> 
- \[2]: <https://www.youtube.com/watch?v=lTRiuFIWV54&t=300sa> 

### Putting the Parts together

I really love [Lofi music][1], and that mean a lot

[1]: <https://www.youtube.com/watch?v=lTRiuFIWV54&t=300s>


# Images
To add an image , add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses. We can also optionally add a title after the URL in the parentheses.

1. Open the file containing the image
2. Adding the image
<br>
    ![This is for testing](moujib-aghrout-s9ESRUFnKDg-unsplash.jpg "This is for testing")
    *Image_caption*
<br>
3. Close the file

### Linking the image

[![This is for testing](moujib-aghrout-s9ESRUFnKDg-unsplash.jpg "This is for testing")](https://www.youtube.com/watch?v=lTRiuFIWV54&t=300s)

# Escaping Character
To display the literal character that would otherwise be used to format text in a Markdown document, add a baclslash (\) in front of the character

\* Without the backslash, this would be a bullet in an unordered list.


# Table
| Testing ID | Testing Amount | Testing Money |
|------------|----------------|---------------|
| 1          | 2              | $20           |
| 2          | 4              | $30           |


# Heading IDs
Adding custome IDs allow you to link directly to heading and modify them with CSS. To add a custome heading ID, enclose the custome ID in curly braces on the same lin as the heading.

[Link to my Testing Heading](#custom-1)

##### My Testing Heading {#custom-1}

# Definition Lists
To create a defininiton list, tupe the erm on the first line. On the the next lien, type a colon followed by a sapce and the definition.

First Term
: This is my Testing first term.  

Second Term
: This is my Testing second term.
: Another Testing


# Strikethrough
We can **strikethrough** words by putting a horizontal line through the center of them.

*Example*: You shouldnot be ~~lazy~~

# Task Lists
- [x] Finish the book
- [ ] Learning ReactJS
- [ ] Learning NodeJS

