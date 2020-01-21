[Class04](https://cassandraortiz.github.io/reading-notes/Class04/class04) \| [Layouts](https://cassandraortiz.github.io/reading-notes/Class04/class04_layout) \| [Functions](https://cassandraortiz.github.io/reading-notes/Class04/class04_functions)  \| [Paired Programming](https://cassandraortiz.github.io/reading-notes/Class04/class04_pairedProgramming)  

# Links

Links are a defining feature of the web, connecting you to another location, page or function to run (like creating an email).

### LINKING to other Sites

**Simple Link**

```html
    <a href="https://cassandraortiz.github.io/reading-notes">READING-Notes</a>
```

**List Links**

```html
<p>Movie Reviews: 
    <ul>
        <li><a href="http://www.empireonline.com"> Empire</a></li>
        <li><a href="http://www.metacritic.com"> Metacritic</a></li>
        <li><a href="http://www.rottentomatoes.com"> Rotten Tomatoes</a></li>
        <li><a href="http://www.variety.com"> Variety</a></li>
    </ul> 
</p>
```

Movie Reviews:
 - [Empire](http://www.empireonline.com)
 - [Matacritic](http://www.metacritic.com)
 - [Rotten Tomatoes](http://www.rottentomatoes.com)
 - [Variety](https://www.variety.com)


**Email Links**

Opens a link with the users perferred email provider TO the address listed.

`<a href="mailto:myemail@example.org">Email Cassy</a>`


**Open Link in New Window**

`<a href="http://www.imdb.com" target="_blank"> Internet Movie Database</a> (opens in new window)`

<a href="http://www.imdb.com" target="_blank"> Internet Movie Database</a> (opens in new window)

---

### LINKING on current website 


Use the file structure tree to call out the reference file. *Reference pg 84 for example*.

| Link Type | Example |
| :-------- | :------ |
| Same Folder | `<a href="reviews.html">Reviews</a>` |
| Child Folder | `<a href="music/listings.html">Listings</a>` |
| Grandchild Folder | `<a href="movies/dvd/reviews.html"> Reviews</a>` |
| Parent Folder | `<a href="../index.html">Home</a>` |
| GrandParent Folder | `<a href="../../index.html">Home</a>` |


**Linking specific parts of a page**

Use the specific element attribute to link on your page. 

```html
<h1 id="top">Film-Making Terms</h1>
<a href="#arc_shot">Arc Shot</a><br />
<a href="#interlude">Interlude</a><br />
<h2 id="arc_shot">Arc Shot</h2>
    <p>A shot in which the subject is photographed by an
    encircling or moving camera</p>
<h2 id="interlude">Interlude</h2>
    <p>A brief, intervening film scene or sequence, not
    specifically tied to the plot, that appears
    within a film</p>
```

Same goes if you are trying to reference a specifc location on another page, just enter in the location...

```html
 <a href="index.html #arc_shot">Arc Shot</a><br />
```

[HOME](https://cassandraortiz.github.io/reading-notes)