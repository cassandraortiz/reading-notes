[Class06](https://cassandraortiz.github.io/reading-notes/Class06/class06) \| [Document Object Model *(pgs 183-242)*](https://cassandraortiz.github.io/reading-notes/Class05/class05_colors) \| [Understanding The Problem Domain Is The Hardest Part Of Programming](https://cassandraortiz.github.io/reading-notes/Class05/class05_text) 

# Object Literals  *(pgs 100-105)*

Objects group together a set of **properties** and **methods** to create a model of a something you would recognize from the real world.

The name of a property is called a **key**.  Keys need to be unique to the object, their values can be datatype.

**Examples:**

```javascript
var hotel = {
    /* These are properties */
    name: Holiday Inn,
    rooms: 220,
    booked: 128,
    /* This is a method */
    CheckAvailablity: function(){
        return this.room - this.booked;
    }
};
```
---

### Accesing an Object and dot notation

dot notation is used by by referencing the object name, followed by ( **.** ) *period*, and then the property name.

` var hotelName = hotel.name;`

Can also reference the property (NOT THE METHOD) by square brackets.

` var hotelName = hotel['name'];`

*this method is commonly used for:*
- name of the property is a number, or 
- the variable is being used in place of the property name.

---

### Literal Notations

You can set the contents of the page with updated information from our object.

```javascript
var hotel = {
    /* These are properties */
    name: 'Holiday Inn',
    rooms: 220,
    booked: 128,

    /* This is a method */
    CheckAvailablity: function(){
        return this.room - this.booked;
    }
};

var elName = document.getElementById('hotelname');
elName.textContent = hotel.name;

var elRooms = document.getElementById('rooms');
elRooms.textContent = hotel.CheckAvailablity();

```

![Literal Notaions Result](/pics/literalNotation.png)

--- 

[HOME](https://cassandraortiz.github.io/reading-notes)




