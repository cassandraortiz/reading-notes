[Class07](https://cassandraortiz.github.io/reading-notes/Class07/class07) \| [Functions, Methods & Objects *(pgs 126-145)*](https://cassandraortiz.github.io/reading-notes/Class07/class07_funcMethObj) \| [Tables](https://cassandraortiz.github.io/reading-notes/Class07/class07_tables)

# Domain Modeling  *([article](https://github.com/codefellows/domain_modeling#domain-modeling))*

Domain modeling is the process of creating a conceptual model in code for a specific problem.  **Object-oriented** models are entities that store data in properties and methods.

The model should verify and validate the understanding of a problem.

***EpicFailVideo***

```javaScript
var EpicFailVideo = function(epicRating, hasAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7,false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

`new` will create a new object with the arguments being stored as the objects properties.

## Generate random number

```javaScript
var EpicFailVideo = function(epicRating, hasAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

EpicFailVideo.protype.generateRandom = function(min, max){
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7,false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1,5));
console.log(corgiFail.generateRandom(1,5));
```

`.prototype` is involked after the object looks through its own objects methods and does not find it.  Using **prototype** to share between two or more objects that share the same code.

## Calculate daily Likes

```javaScript
var EpicFailVideo = function(epicRating, hasAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max){
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

EpicFailVideo.prototype.dailyLikes = function(){
    var viewers, percentage;
    viewers = this.generateRandom(10,30) * this.epicRating;

    if (this.hasAnimals){
        percentage = 0.75;
    } else {
        percentage = 0.40;
    }
    return Math.round(viewers * percentage);
}

var parkourFail = new EpicFailVideo(7,false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.dailyLikes());
console.log(corgiFail.dailyLikes());
```

this example creates a new `.prototype.function` without any arguments, but sets new properties within it to extract information for the shared objects.

when creating further prototype fucntions for the shared object, simply call them through the `this.dailyLikes()`

---

[HOME](https://cassandraortiz.github.io/reading-notes)