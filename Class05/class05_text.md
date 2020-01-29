[Class05](https://cassandraortiz.github.io/reading-notes/Class05/class05) \| [Images *(pgs 94-125)*](https://cassandraortiz.github.io/reading-notes/Class05/class05_images) \| [Colors *(pgs 246-263)*](https://cassandraortiz.github.io/reading-notes/Class05/class05_colors) 

# Text  *(pgs 264-299)*

2 Groups of Properties that can effect text apperance
1. Direct Effect the font and the appearance (typeface, size)
2. Same effect on text, no matter the font (color, spacing)

### Typeface 

Understanding the different terminology:
- **Serif** - extra details on the ends of the main strokes of the letters (used in long text, easier to read)
- **Sans-Serif** - straight ends to letter (much cleaner design)
- **Monospace** - every charachter is the same fixed width (Makes code/text easier to follow)

Appearance to typeface:
- **Weight** - [Light, Medium, Bold, Black] 
- **Style** - [Normal, Italic, Oblique] 
- **Stretch** - [Condensed, Regular, Extended] 

--- 

### Font-Family
[(Font-Family CheatSheet)](https://www.w3.org/Style/Examples/007/fonts.en.html)

Font Sources: [fontsquirrel](https://www.fontsquirrel.com) \| [fontex](https://www.fontex.org) \| [openfontlibrary](https://www.openfrontlibrary.org) \| [typekit](https://www.typekit.com)  \| [kernest](https://www.kernest.com)  \| [fontspring](https://www.fontspring.com) \| [webfonts](https://www.google.com/webfonts)

- **font-size** - [pixels, percentages, ems] *em* is equivalent to width of a letter m.

- **font-face** - use a font a user doesnt have by downloading it
```css
@font-face {
    font-family: 'ChunkFiveRegular';
    src: url('fonts/chunkfive.eot');
}
h1 {
    font-family: ChunkFiveRegular, Georgia, serif;
}
```

- **font-weight** - [normal, bold]

- **font-style** - [normal, italic, oblique]

---

### Text Properties

- **text-transform** - [uppercase, lowercase, capitalize]

- **text-decoration** - [none, underline, overline, line-through, blink (animates text flash on/off)]

- **line-height** *(leading)* - vertical space between lines of text

- **letter-spacing** *(kerning)* - space between each letter

- **word-spacing** - spaces between each word (should be defined in *em*)

- **text-align** - [left, right, center, justify (every line except the last takes up the full width of element)]

- **vertical-align** - [baseline, sub, super, top, text-top, middle, bottom, text-bottom] - does not effect vertical alignment, used more with inline elements (like images)

- **text-indent** - only effects the first line

- **text-shadow** - three conditions: (how far to left/right shadow should fall, distance top/bottom shadow should fall, *optional* amount of blur, color)
```css
p{
    text-shadow: 2px 2px 7px #111111;
}
```

### Psuedo-Elements
Lets you select specific sections of an element.

- **:first-letter** / **:first-line** 
- **:link** / **:visited** / **:hover** / **:active** / **:focus** 


### Attribute Selectors
rules that apply to elements that have attributes with specific values

| Selector | Meaning | Example |
| :------- | :------ | :------ |
| `EXISTENCE` | `[]`<BR /> Matches a specifc attribute (whatever it is) | `p[class]`<br/>Targets and `<p>` element with an attribute called class|
| `EQUALITY` | `[-]`<br/> Matches a specific attribute with a spcific value | `p[class="dog"]`<br/> Targets andy `<p>` element with an attribute called class whose value is dog|
| `SPACE` | `[~=]`<br/> Matches a specific attribute whose value appears in a space-seperated list of words | `p[class~="dog"]` Targets any `<p>` element whoes value is a list of space-separated words, one of which is dog |
| `PREFIX` | `[^=]`<br/> Matches a specific attribute whose value begins with a spcific string | `p[attr^="d"]` Targets any `<p>` element with an attribute whose value begins with the letter "d"|
| `SUBSTRING` | `[*=]`<br/> Matches a specific attribute whose value contains a specific substring | `p[attr*"do"]` Targets any `<p>` element with an attribute whose value contains the letters "do"|
| `SUFFIX` | `[$=]`<br/> Matches a specific attribute whose value ends a specific substring | `p[attr$"g"]` Targets any `<p>` element with an attribute whose value ends with the letter "g"|

---

[HOME](https://cassandraortiz.github.io/reading-notes)
