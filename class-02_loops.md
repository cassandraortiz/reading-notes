[Class-02](https://cassandraortiz.github.io/reading-notes/class-02.md) \| [HTML-Text Cheat Sheets](https://cassandraortiz.github.io/reading-notes/class-02_html-text.md) \| [Introducing CSS](https://cassandraortiz.github.io/reading-notes/class-02_CSS-intro.md) \| [Introducing JavaScript](https://cassandraortiz.github.io/reading-notes/class-02_java-intro.md)

# CONDITIONAL STATEMENTS

## IF Statements

IF Statements evaluates a condition.  If that condition is `true`, it will complete the proceeding code.

![IF Statement](/pics/IfStatement.JPG)

Example:

```JavaScript
var age = 26;
var msg;

if (age >= 21){
    msg = 'You are old enough to drink!'
}
```

IF/ELSE Statements evaluates a condition.  If that condition is `true`, it will complete the proceeding code. If condition is `false` it will complete the second code block.

![IF../ELSE.. Statement](/pics/IfElse_Statement.JPG)

Example:

```JavaScript
var age = 26;
var msg;

if (age >= 21){
    msg = 'You are old enough to drink!'
} else {
    msg = 'You are NOT old enough to drink!'
}

```

# LOOPS

A Loop is exactly what it sounds like, the code will keep going around and around until a condition is met. 

 - **break** causes termination of the loop and goto the next statement outside the loop.

 - **continue** continue with the current code and check the condition again.


#### REMEMBER: Browser stops what its doing when it reaches a loop, and will continue until that condition is met!  

be careful not to get into a **infinite loop**, where it will never give you a _false_ result to continue.

---

## FOR Loops

For loops will continue through an array of items, with a specific starting/stopping values.  These values are stored as variables and will loop through in given incremints until the stopping value is met. 

```JavaScript
var drinks = ['vodka', 'rum', 'tequila'];
var arrayLength = drinks.length; 
var roundNumber = 0;
var msg = '';

for(var x=0; x < drinks;x++){
    roundNumber = (x+1);
    msg += 'He had: ' + roundNumber + 'drinks ';
    msg += drinks[x] + '<br />';
}
document.getElementById('answer').innerHTML = msg;
```

Result: 
```Javascript
Round 1: He had: 1 drinks
Round 2: He had: 2 drinks
Round 3: He had: 3 drinks
```


## WHILE Loops

While loops will continue through a loop until a certain criteria is meet. 

```JavaScript
var p = 1;
var msg = '';

while(p<10){
    msg += p + ' x 5 = ' + (p*5) + '</br>';
    i++;
}
document.getElementById('answer').innerHTML = msg;
```

Result: 
```Javascript
1 x 5 = 5
2 x 5 = 10
3 x 5 = 15
4 x 5 = 20
5 x 5 = 25
6 x 5 = 30
7 x 5 = 35
8 x 5 = 40
9 x 5 = 45
```
---

[HOME](https://cassandraortiz.github.io/reading-notes/README.md)