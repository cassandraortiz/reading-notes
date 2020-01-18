[Class03](https://cassandraortiz.github.io/reading-notes/Class02/class-02) \| [Lists](https://cassandraortiz.github.io/reading-notes/Class03/class03_Lists) \| [Boxes](https://cassandraortiz.github.io/reading-notes/Class03/class03_Boxes) \| [Learning Journal](https://cassandraortiz.github.io/reading-notes/Class03/class03_journal)


# DECISIONS
## Switch Statements

switch statements selects each *case* of a variable and completes proceeding code when condition is met.  Similar to the If..then..else, but with less code.

```Javascript
switch (MarvelMen){
    case 'Iron Man':
        msg = 'Smartest Avenger';
        break;
    case 'Thor':
        msg = 'Point Break'
        break;
    case 'Captain America':
        msg = 'Language!';
        break;
    default:
        msg = 'Marvel Rules, DC sux!';
        break;
}
```
`break;` tells JavaScript that it has finishe with that statement.

---

## `use strict`

Using `use strict` at the beginning of our JavaScript code, will force the user to evaluate both value and data type doing a comparison.


### TRUTHY & FALSY

**Truthy** are values that are treate *as if* they were true (1)

**Falsy** are values that are treate *as if* they were false (0)

*See [Intro to JavaScript](https://cassandraortiz.github.io/reading-notes/Class02/class-02_java-intro) for more info on Logical Operators*

---
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

## DO WHILE loops

the difference between DO WHILE and WHILE loops is that the statement comes before the codition.

```JavaScript
var p = 1;
var msg = '';

do {
    msg += p + ' x 5 = ' + (p*5) + '</br>';
    i++;
} while(i < 1);

document.getElementById('answer').innerHTML = msg;
```

Result: 
```Javascript
1 x 5 = 5
```

---

[HOME](https://cassandraortiz.github.io/reading-notes)