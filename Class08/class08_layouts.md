[Class08](https://cassandraortiz.github.io/reading-notes/Class08/class08) \| [Class04-Layouts](https://cassandraortiz.github.io/reading-notes/Class04/class04_layout)

# Layouts  

For the basic understanding of layouts, checkout [Class04-Layouts](https://cassandraortiz.github.io/reading-notes/Class04/class04_layout)

## CSS Float

**Float** places boxes next to each other. The height of the object effects where the item will be placed.  

The **clear** property, no element (in containing element) should touch the left/right sides of the box.

 `clear: (left/right/both/none);`

### Multi-Column Layouts

`<div>` elements are setup to create the *column*. set the following properties to position the columns next to each other:

```css
.column1of3, .column1of2, .column3of3 {
    width: 300px;
    float: left;
    margin: 10px;
}
```

---

## Screen Sizes

screen sizes vary per device and can show different amounts of information. Here's a [link](https://www.responsivedesignchecker.com/) for a responsive design checker.

Because resolution changes so much, web designers create pages between **960-1000** pixels wide.

The height is hard to figure, so most designers try to put information within the first **570-600** pixels.

---

## Types of Layouts

### Fixed Width Layout

The fixed width layout will stay the same width no matter what size the browser window is

**Advantagegs**:

- Pixel values are accurate
- designer has greater control
- control lengths of lines
- image size will remain the same.

**Disadvantages**:

- end up with big gaps around pages
- if user resolution higher, appearance can be smaller
- user increase font size, text may not fit
- works best on similar designed resolution screens
- could take more vertical room.

### Liquid Width Layout

Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

**Advantagegs**:

- Pages expand to fill entire browser window
- page can contract to fit without user scrollin
- user can use larger font sizes

**Disadvantages**:

- If you dont control the width, design can look different than expected.
- If user has a wide window, lines can get longer/harder to read.
- User has narrow window, text can look squished.
- if image in fixed width is too small, it can overflow the text.

### Grid Layout

Grids set consistent proportions and spaces between items which helps to create a professional looking design.

Standard box sizes of: 940, 460, 300, 220 or 140 pixels

With margins set to 10px.

---

## Multiple Style Sheets

Some designers create separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site.  

To add multiple sheets to a page:


1. In the HTML you can use a separate <link> element for each style sheet.

2. Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.

```css
 @import url("tables.css");

 body{
     color: #666666;
     background-color: $f8f8f8;
     text-align: center;
 }
```

---

[HOME](https://cassandraortiz.github.io/reading-notes)