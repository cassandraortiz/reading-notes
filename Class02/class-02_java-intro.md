[Class-02](https://cassandraortiz.github.io/reading-notes/Class02/class-02) \| [HTML-Text Cheat Sheets](https://cassandraortiz.github.io/reading-notes/Class02/class-02_html-text) \| [Intro to CSS](https://cassandraortiz.github.io/reading-notes/Class02/class-02_css-intro) \| [Loops](https://cassandraortiz.github.io/reading-notes/Class02/class-02_loops) \| [Learning Journal](https://cassandraortiz.github.io/reading-notes/Class02/class-02_journal)

# INTRODUCTING JavaScript

Javascript is the programming language that puts dynamic and interactive experiences on the webpage. 

**Statements** are individual instructions or steps, each statement starts on a new line. Statements should end with a semicolon `;`
some statements uses curly brackets to place the code inside known as **code blocks**.  These statements do not require a semicolon. 

**Variables** are bits of stored information. It is not required to establish what type of variable you are declaring (i.e. Number, string, boolean)

```JavaScript
var x = 2;
var y = 3;
var z = x*y;
z = 6
```

**Comments** help you and others understand what your code is doing.  
 `// single line comment` <br />  `/* multiple line comment`

**Data Types** distinguish between different values types

 - ***Numeric Data Type*** - handles all number `0.98992`

 - ***String*** - text that consists of letters and other charachters `'Hi friend!`

 - ***Boolean*** - true or false values only

Use both the single `' '` and `" "` double quotes to assign a string.  It has to be the same opening/closing, ` 'text"` is invalid.

***Escaping*** is the use of a backwards slash `/` before any type of quete mark that appears within a string 

```Javascript
var a = 'Your mom said /"Hello!/"'
```

---

### MULTIPLE WAYS TO ASSIGN VARIABLES

```Javascript
var price = 5;
var quantity = 14;
var total = price * quantity;
```

```Javascript
var price, quantity, total;
price = 5;
quantity = 14;
total = price * quantity;
```

```Javascript
var price = 5, quantity = 4;
var total = price *quantity;
```

```Javascript
var el = document.getElementById('cost');
el.textContent = '$' + total;
```
*This is variable is holding a refernce to an element on the HTML page.*

### **!! ALWAYS FOLLOW THESE RULES FOR NAMING VARIABLES !!**

1. Name MUST begin with a letter, dollar sign ($) or underscore(_)
2. Names can only contain: letters, numbers, dollar signs or underscors.  ***Never use dash (-) or dot (.)***
3. Can NOT use **keywords** or **reserved** words.  These are special words JavaScript uses to interpert or do something.
4. variables are ***case sensitive***, try not to use the same name with different cases - it's bad practice.
5. Use a name that describes the info of the variable
6. If name is more than one word, use a capital letter for the first letter of the second word: _firstName_

---

## ARRAYS

An array stores a list of values within its variabled
- the values of the list are stored inside square brackets`[]`
- each value is seperated by a comma
- values do not need to be the same data type

**array literal** _*Preferred Method_

``` Javascript
var colors = ['white','blue','pink'];
```

**array constructor** 

_Note:_values are stored in parethesis (not squared brackets)_

``` Javascript
var colors = new Array('white',
                        'blue',
                        'pink');
```

##### Accessing Items

```javascript
var colors; 
colors = ['white','blue','pink']
```
- Values in an array are accessed as index, 0 being the first.

INDEX | VALUE
----- | -----
0 | white
1 | blue
2 | pink

- find the value of specific item of arry
```javascript
var itemtwo
itemtwo = colors[2];
```
- find the number of items in an array
```javascript
var numColors
numColors = colors.length
```
- change the value of a specific item in array
```javascript
colors[2] = 'puce'
```
--- 

## OPERATORS

### **Comparison Operations**

You can evaluate situations by comparing one value to what you would expect it to be.  The result will be a Boolean `true` or `false`.


Operator | Compares two values to see if... | Example
-------- | ----------- | -------
== | they are the same | `"Hello" == "Goodbye"` returns _false_  : `"Hello" == "Hello"` returns _true_
!= | they are _NOT_ the same | `"Hello" != "Goodbye"` returns _true_  : `"Hello" == "Hello"` returns _false_
=== |  _both_ data type and value are the same | `"55" === 55` returns _false_  : `55 === 55` returns _true_
!== |  _both_ data type and value are _NOT_ the same | `"Hello" != "Goodbye"` returns _true_  : `"Hello" == "Hello"` returns _false_
\> | left value is greater than the right value | `89 > 63` _true_  :  `63 > 89` _false_
\>= | left value is greater than OR Equal to the right value | `89 >= 63` _true_  :  `63 >= 63` _true_  :  `63 >= 89` _false_  
< | left value is less than the right value | `89 < 63` _false_  :  `63 > 89` _true_
<= | left value is less than OR Equal to the right value | `89 <= 63` _false_  :  `63 <= 89` _true_  :  `63 <= 63` _true_


### **Logical Operations**

You can compare the results of more than one value.  The result will be a Boolean `true` or `false`.


Operator | What does it Test? | Example
-------- | ----------- | -------
&& | (AND) test multiple values - ALL values need to be _true_ for result to be _true_ | (`_true_`,`_true_`) = `_true_` : (`_true_`,`_false_`) = `_false_` : (`_false_`,`_true_`) = `_false_` : (`_false_`,`_false_`) = `_false_`
\|\| | (OR) test multiple values - ANY value needs to be _true_ for result to be _true_ | (`_true_`,`_true_`) = `_true_` : (`_true_`,`_false_`) = `_true_` : (`_false_`,`_true_`) = `_true_` : (`_false_`,`_false_`) = `_false_`
! | (NOT) takes a single boolean value and inverts it | !_true_ = `_false_` : !_false_ = `_true_`

---

[HOME](https://cassandraortiz.github.io/reading-notes)
