[Class06](https://cassandraortiz.github.io/reading-notes/Class06/class06) \| [Document Object Model *(pgs 183-242)*](https://cassandraortiz.github.io/reading-notes/Class06/class06_objectLiterals) \| [Understanding The Problem Domain Is The Hardest Part Of Programming](https://cassandraortiz.github.io/reading-notes/Class06/class06_article) 

# Document Object Model *(Chapt 5; pgs 183-242)*

DOM specifies how browsers should create an HTML page and how JavaScript can access/update the window.  It is NOT part of html or JavaScript.

**API** (*Application Programming Interface*) is also used to reference the DOM.  API's let programs talk to each other. 

![DOM TREE](https://www.w3schools.com/js/pic_htmltree.gif)

Each object with methods & propoperties is called a ***Node***.

- **Document Node** - represents the entire page, the starting point for all visits to the DOM tree.
- **Element Node** - relates to the html elements, looking at those element first, then can access the attribute/text nodes.
- **Attribute Node** - are part of the element, like the class/id.
- **Text Node** - elements that contains text. These nodes can not have a child element.

---
 
## Working with DOM Tree

To access the DOM tree, you need to *select the node* and *use its content*

### Step 1 - Access the Element

**DOM query** - select one or multiple elements

`getElementById()` | uses the value of the elements id attribut( unique)

`querySelector()` | Uses a CSS selector, returns first matching element.

`getElementByClassName()` | selects all elements with class name

`getElementsByTagName()` | selects all elements with specific tag name

`querySelectorAll` | matches all css selector elements

**Traversing** - moving from one element to another

`parentNode` | Selects the parent of the current element node (returns just one)

`previousSibling / nextSibling` | Selects the previous or next sibling from the DOM tree

`firstChild / lastChild` | Select the first/last chald of the current element.

### Step 2 - Work with the Element

**Access / Update Text Nodes**

`nodeValue` | Text nodes ONLY property to get the text value.


**Work with HTML content**

`innerHTML` | allows access to child elements and text content.

`textContent` | selecting text content

`createElement` `createTextNode` `appendChild()` `removeChild()`| methods to create or manipulate elements.

**Access or update Attribute Values**

`className/id` | updates the value of class/id attributes

`hasAttribute` | checks if attribute exists

`getAttribute` | gets attribute value

`setAttribute` | updates the attribute value

`removeAttribute` | removes an attribute

---

## NodeList: DOM queries

NodeLists are a collection of element nodes, each node is given an index number [0].

**Live NodeList** - when the script updates the page, so does your NodeList.  These are usually faster to generate.

**Static NodeList** - when the script updates the page,the NodeList does not updated to refelect the changes made by the script.


**Selecting elements from a nodeList**

`item()`| this will select the index of the item 

```javascript
var elements - document.getEdlementByClassName('hot')
if (elements.lenght >= 1) {
    var firstItem = elements.item(0);
}
```


--- 

[HOME](https://cassandraortiz.github.io/reading-notes)

