[Class10](https://cassandraortiz.github.io/reading-notes/Class10/class10) 

# Debugging

Order of execution can cause issues.  Functions within functions or "stacking" will result in an error if one of the containing funtions has an error.

***Hoisting*** or the concept of the two step process of Preparing and then Executing the code. 

## Built in Errors

| Object | Description |
| :----- | :---------- |
| `Error` | Generic Error - the other errors are all based upon this error |
| `SyntaxError` | Syntax has not been followed |
| `ReferenceError` | Tried to reference a variable that is not declared/within scope |
| `TypeError` | An unexpected data type that cannot be coerced |
| `RangeError` | Numbers not in acceptable range | 
| `URIError` | encodeURI(), decodeURI(), and similar methods used incorrectly |
| `EvalError` | eval() function used incorrectly |

All errors will show the following information: 

- name
- message
- fileNumber
- lineNumber


**Use the Browsers Inspector Dev Tools to help with Errors**

### Console Methods

- `console.log` 
- `console.info()` - used for general information
- `console.warn()` - used for warnings
- `console.error()` - holds errors
- `console.group()` - expandable group with other console. listed inside.
- `console.table()` - output a table showing object/arrays

### Handling Exceptions - try,catch, finally

---

[HOME](https://cassandraortiz.github.io/reading-notes)