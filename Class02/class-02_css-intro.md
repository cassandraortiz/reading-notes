[Class-02](https://cassandraortiz.github.io/reading-notes/Class02/class-02) \| [HTML-Text Cheat Sheets](https://cassandraortiz.github.io/reading-notes/Class02/class-02_html-text) \| [Introducing JavaScript](https://cassandraortiz.github.io/reading-notes/Class02/class-02_java-intro) \| [Loops](https://cassandraortiz.github.io/reading-notes/Class02/class-02_loops) \| [Learning Journal](https://cassandraortiz.github.io/reading-notes/Class02/class-02_journal)

# INTRODUCTING CSS (Cascading Selector Sheets)

Remember our Sitemap we designed?  All those boxes within boxes and so on.  Well, now its time to design those boxes ***Elements*** and make them look pretty! CSS files keep our web pages smaller and reduces the amount of repetative code.

### **Understanding the different Elements**

ELEMENT | WHAT TO KNOW | EXAMPLES
------- | ------------ | --------
BLOCK | look like they start on a new line | \<h1>, \<h6>, \<p>, \<div>
INLINE | flow within the text and do not start on a new line | \<b>, \<i>, \<img>, \<em>, \<span>

---
## RULES

### A CSS rule contains 2 parts: `p {font-family: Arial;}`

**Selector** - indicates which HTML element the rule applies to.  You can have multiple elements seperated by commas ` html, body {color: red;}`

**Declarations** - indicate how the elements should be styled.  Declarations are seperated by `;` Declarations also have 2 parts:

  - **properties** - indicate the aspect of the element you want to change

  - **values** - specify the settings you want to use

---
## SELECTORS

### **Internal Selectors**

Selector | Meaning | Example
---------| ------- | -------
Universal | applies to all elements | `* {}`
Type Selector | mathes element name | `h1, h2, h3 {}`
Class Selector | matches class attribute | `.note{}`  `p.note{}` targets only \<p>elements with that class
ID Selector | matches the id attributes | `#introduction {}`
Child Selector | direct child of another | `li>a {}` targets any \<a> element that are children of \<li>
Descendant Selector | descendent of another specified element (not just direct child) | `p a {}` targets and \<a> element that site inside the \<p> element
Adjacent Sibling Selector | the next sibling of another | `h1+p {}` targets the first \<p> after any \<h1> (but not others)
General Sibling Selector | Sibling of another, does not have to be directly preceding | `h1~p {}` If you had 2 \<p> elements that are siblings of \<h1> element, it applies to both

---

### **External Selectors** `<link>`


**href:** specifies the path to link (css file location)

**type:** type of document being placed (text/css)

**rel:** relationship between HTML and the linked file.

``` html
<html>
    <head>
        <title> Quick Example </title>
        <link href="css/styles.css" type="text/css" rel="stylesheet"/>
    </head>
    <body>
        <h1> Look at me! </h1>
        <p> Hey there, it looks like we're figuring it out!</p>
    </body>
</html>
```
``` css
 body{
     font-family: arial;
     background-color: rgb(164,184,180);
 }
 h1{
     color: magenta;
 }

```
---

#### UNDERSTANDING CSS

- **LAST RULE:** If two idential selectors are used, the last iterance of the code will take precidence. 
- **SPECIFICITY:** The more specific selector will take precidence.
- **INHERITANCE:** Properties that will pass down to the child element (ex. font-family, colors)
- **IMPORTANT**: You can add `!important` after any property to more important than other rules

---

[HOME](https://cassandraortiz.github.io/reading-notes/README.md)
