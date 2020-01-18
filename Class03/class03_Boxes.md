[Class03](https://cassandraortiz.github.io/reading-notes/Class02/class-02) \| [Lists](https://cassandraortiz.github.io/reading-notes/Class03/class03_Lists) \| [Descisions & Loops](https://cassandraortiz.github.io/reading-notes/Class03/class03_DescisionsLoops) \| [Learning Journal](https://cassandraortiz.github.io/reading-notes/Class03/class03_journal)

# Boxes

### Sizing
You can control the size of your element with ***width*** and ***height*** property setting.  ***max-**** property will stretch the element box across or down the browser window. ***min-**** will limit the size of the box element on the window.

### Overflow

If the content is too big for the box, the ***overflow*** property. 

***overflow: hidden;*** will hide the extra content ***overflow: scroll;*** adds a scroll bar to see the missing content.

---

### Border / Margin / Padding

***Margin*** the outside edge around the border. Setting the margin will give a gap from the next boxes border.

![Border/Margin/Padding](/pics/css-box-model.png)

***Border*** the actual box around the element. The border serarates the edges of one box from another.   You can also set the ***border-style***, to give different effects.  Additionally, you can give the border a ***color***.

![border-style](/pics/lineStyles.png)

***Padding*** the space between the border and the inside content.

#### Setting the sizes: 

All settings, if not specifically specified will be listed in the following order: 

 *TOP - RIGHT - BOTTOM - LEFT*

 ` margin: 1px 2px 3px 4px`

### Display Properties...

`display: inline;` - displays text in same line

`display: block;` - displays inline elements as blocks

`display: inline-block;` - displays block level elements as inline 

---
### Additional Properties
---
##### border-image:
To specify border-image by the following:
  1. An image to use as the border
  2. where to slice the image *(9 section box - think tic-tac-toe)*
  3. what to do with edges *(stretch, repeat, round)*

```css
p{
    border-image: url("images/circle.jpg") 25% stretch;
}
```
---
##### box-shadow:
Adds a drop shadow around the box needs to have the offsets atleast of the following values:
1. Horizontal offset
2. Vertical offset
3. Blur Distance
4. Spread of Shadow

```css
p{
    box-shadow: inset 0 0 10 5 #777777;
}
```
---
##### border-radius:
can specify the individual corners of each box

- border-top-right-radius
- border-bottom-right-radius
- border-bottom-left-radius
- border-top-left-radius

```css
p{
    border-radius: 5px 5px 5px 5px;
}
```

to achieve an elliptical-shape the distances fo the horizontal and vertical parts. 

```css
p{
    border-top-right-radius: 80px 50px;
}
```


---

[HOME](https://cassandraortiz.github.io/reading-notes)






<!--
Referenced for pictures:
 https://sabe.io/classes/css/css-box-model-padding-border-margin
 https://flaviocopes.com/css-border/
 https://css-tricks.com/understanding-border-image/
