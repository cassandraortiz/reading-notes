[Class07](https://cassandraortiz.github.io/reading-notes/Class07/class07) \| [Tables *(pgs 126-145)*](https://cassandraortiz.github.io/reading-notes/Class07/class07_tables) \| [Domain Modeling](https://cassandraortiz.github.io/reading-notes/Class07/class07_article)

# Functions, Methods and Objects  *(pgs 106-144)*

## Object Constructors

Object constructors can use a function as a *template* for creating objects.

**Example Template**

```JavaScript
function Hotel(name, rooms, booked){
    this.name = name;
    this.rooms = rooms;
    this.booked = booked;
    this.checkAvailability = function(){
        return this.rooms - this.booked;
    }
}
```

*Adding a new item:*

```
var quayHotel = new Hotel('Quay', 40, 25);
```

You can combine arrays and objects to create complex data structures.

## Built-In Objects
[resources](https://javascriptbook.com/resources)

**Browswer Object Model**

![BrowswerObjectModel](../pics/Browser&#32;Object&#32;Model.png)

| Property | Description |
| :------- | :---------- |
| `window.innerHeight` | Height of window (excluding browser chrome/user interface)(in pixels) |
| `window.innerWidth` | Width of window (excluding browser chorme/user interface)(in pixels)
| `window.pageXOffset` | Distance document has been scrolled horizontally (in pixels) |
| `window.pageYOffset` | Distance document has been scrolled vertically (in pixels) |
| `window.screenX` | X-coordinate of pointer, relative to top left corner of screen (in pixels) |
| `window.screenY` | Y-coordinate of pointer, relative to top left corner of screen (in pixels) |
| `window.location` | Current URL of window object (or local file path) |
| `window.document` | Reference to document object, which is used to represent the current page contained in window |
| `window.history` | Reference to history object for browser window or tab, which contains details of the page that have been viewed in that window or tab |
| `window.history.length` | Number of items in history object for browser window or tab |
| `window.screen` | Reference to screen object |
| `window.screen.width` | Accesses screen object and finds value of its width property (in pixels)|
| `window.screen.height` | Accesses screen object and finds value of its height property (in pixels)|

| Method | Description |
| :----- | :---------- |
| `window.alert()` | Creates dialog box with message (user must click OK button to close it)|
| `window.open()` | Opens new browser window with URL specified as parameter (if browser has pop-up blocking software installed, this method may not work)|
| `window.print()` | Tells browser that user wants to print contents of current page (acts like user has clicked a print option in the browser's user interface)