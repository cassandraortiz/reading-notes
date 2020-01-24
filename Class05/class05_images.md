[Class05](https://cassandraortiz.github.io/reading-notes/Class05/class05) \| [Colors *(pgs 246-263)*](https://cassandraortiz.github.io/reading-notes/Class05/class05_colors) \| [Text *(pgs 264-299)*](https://cassandraortiz.github.io/reading-notes/Class05/class05_text) 

# Images  *(pgs 94-125)*

Great images help make the difference between average and engaging sites.

Images should: 
- be Relevant
- Convey Information
- Convey the Right mood
- Be instantly recognizable
- Fit the color palette

Stock Photo Sites:  [istockphoto](https://www.istockphoto.com/) \| [gettyimages](https://www.gettyimages.com/) \|  [veer](https://www.veer.com/) \|  [sxc](https://www.sxc.com/) \|  [fotolia](https://www.fotolia.com/)

Store site images in folder called ***images***.  Can always add subfolders for larger sites called ***interface*** or ***products***.

## Adding Images

`<img src="/pics/smiley.jpg" alt="smiling sloth" title="Happy Little Sloth"/>`

 - `src` - tells where the image is located
 - `alt` - accesibility tag - describing image for blind users
 - `title` -  tag shown when hover over image

### Image Placement

- IMAGE BEFORE PARAGRAPH

```html
<img src="/pics/smiley.jpg" alt="smiling sloth" width="100"/>
<p> Isn't this sloth just the cutest little thing? He wants to tell you a joke... What do you call a three-humped camel?? ... Pregnant! .... Ha-ha-Ha~!</p>
```
![ImageBefore](/pics/ImageBefore.png)

- IMAGE INSIDE PARAGRAPH

```html
<p><img src="/pics/smiley.jpg" alt="smiling sloth" width="100"/> Isn't this sloth just the cutest little thing? He wants to tell you a joke... What do you call a three-humped camel?? ... Pregnant! .... Ha-ha-Ha~!</p>
```
![ImageInside](/pics/ImageInside.png)

- IMAGE IN MIDDLE OF PARAGRAPH

```html
<p>Isn't this sloth just the cutest little thing? He wants to tell you a joke... What do you call a three-humped camel?? ... <img src="/pics/smiley.jpg" alt="smiling sloth" width="100"/> Pregnant! .... Ha-ha-Ha~!</p>
```
![ImageMiddle](/pics/ImageMiddle.png)

- HORIZONTAL ALIGNMENT (LEFT & RIGHT)

```html
<p><img src="/pics/smiley.jpg" alt="smiling sloth" width="100" align="left"/> Isn't this sloth just the cutest little thing? He wants to tell you a joke... What do you call a three-humped camel?? ... Pregnant! .... Ha-ha-Ha~!</p>
```
![Align Horizontal](/pics/AlignHoriz.png)


- VERTICAL ALIGNMENT (TOP / MIDDLE / BOTTOM)

```html
<p><img src="/pics/smiley.jpg" alt="smiling sloth" width="100" align="middle"/> Isn't this sloth just the cutest little thing? He wants to tell you a joke... What do you call a three-humped camel?? ... Pregnant! .... Ha-ha-Ha~!</p>
```
![Align Vertical](/pics/AlignVert.png)

*- this places the starting text line in the middle of the image*

*- if you want text to wrap around the image, use float*


- FIGURE CAPTION
```html   
<figure>
<img src="/pics/smiley.jpg" alt="smiling sloth" width=100%/>
<br />
<figcaption> Just a happy little sloth!</figcaption>
</figure>
```
![Caption](/pics/caption.png)

---

## Three Rules for Creating Images

1. Save Images in the Right Format
2. Save Images at the Right Size
3. Use the correct Resolution

Online Editors:  [photoshop](https://www.photoshop.com/) \| [pixlr](https://www.pixlr.com/) \|  [splashup](https://www.splashup.com/) \|  [ipiccy](https://www.ipiccy.com/) 

### Formats

*.jpg* - colored pictures (many pixels)

*.gif* / *.png* - images with few colors (flat color); such as logo, illustrations and diagrams.

**Image resolution** - Images created for the web, should have a resolution of: **72 ppi**.  Large images increase size of the file.

*.svg* - vector images - images with transparent backgrounds

*GIFs* - animated gifs, (ex. spinning wheel) should only be used for simple illustrations. 

---

[HOME](https://cassandraortiz.github.io/reading-notes)


<!--Picture used from:  https://www.pinterest.com/pin/459789443202656510/ -->

