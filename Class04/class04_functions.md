[Class04](https://cassandraortiz.github.io/reading-notes/Class04/class04) \| [Links](https://cassandraortiz.github.io/reading-notes/Class04/class04_links) \| [Layouts](https://cassandraortiz.github.io/reading-notes/Class04/class04_layout) \| [Paired Programming](https://cassandraortiz.github.io/reading-notes/Class04/class04_pairedProgramming)  

# Functions

Functions let you group a series of statements toghether to perform the tasks.  You are able to reuse functions multipe time throught  your code. 

**Calling** a function, when you ask computer to perform the function.  This call is placed in your code block, at the point where you want to execute the task. 

At that point, the computer will read the code.  Sometimes we will need to provide information to the function, which is called **parameters**.  If you wish that the function provide information back, this will need a **return value**.  

```javascript
function byeFelicia(){
    document.write('Bye Felicia!');
}
```

```javascript
function getBAC(drinks){
    var bac = drinks * 0.02;
    return bac;
}
```
```javascript
var ActualBAC = getBAC(6);
```
`ActualBAC = 0.12`

**Arguements are the actual values passed into the parameters of the function (i.e. 6)**

- in our hmtl we will need to establish our javascript file - in the Head, before we call our function in our code block


## Multiple Values out of a Function

You are able to use arrays within functions.  You reference the functions index number to get the specific result.

```javaScript

function getSize(width, height, depth){
    var area = width * height; 
    var volume = width * height * depth;
    var size = [area, volume];
    return sizes;
}
var areaOne = getSize(3,2,3)[0];
var volumeOne = getSize(3,2,3)[1];
```
 
 A ***function declaration*** creates a function you can call later, also known as a *named function*.

 A ***fuction expression*** the name is omitted and usually treated as an expression, also known as *anonymous function*.

[HOME](https://cassandraortiz.github.io/reading-notes)