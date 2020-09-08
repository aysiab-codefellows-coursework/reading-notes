# Class 07: Reading Assignment 07
*Sections read:* 
- [This Article](https://github.com/codefellows/domain_modeling#domain-modeling)
- Ch. 6 (HTML&CSS)
- Ch. 3 (JavaScript&JQuery)

### ABC's of Object Base Programming
*An article by: Aysia Brown*

Object Based Programming is fundamental for any programmer to learn and get a firm grasp on. This methodology is used universally among programmers across many languages. Objects are a set of grouped together functions, and variables called ***methods and properties***. 

In [Read 06](read-06.md), the quiz mentions how to make objects literally. Even better we can also use constructor functions. 

Constructor functions are functions that are used to construct objects. Below is an example of what an constructor function looks like. In this example, the constructor function is used to create objects that contain information about adoptable pets for a shelter. 
```
var PetListing = function(name,age,species,breed) {
    this.name = name;
    this.age = age;
    this.species = species;
    this.breed = breed;
}
```
`this` keyword refers to the property or method distinctly in *this* object.  

Just a way of convention, but object constructors are often functions that start with a capital letter. Also notice that rather than in literal function every statement ends with a `;` rather than a `,`. 

The constructor function saves time and is cleaner rather than initializing a sepearate object for each and every pet listing. However, let's say we want to construct a new instance of this object for a new pet named Iggy. 
```
var iggy = new PetListing("Iggy","4 years", "Dog","Boston Terrier");
```
`new` is an important keyword that describes that we are creating a new instance of the object and storing it within our new variable iggy. 

Did you know that built in objects that are available to your disposal? 

They are:
- **Browser Object Model:** creates a model for the browser tab or window. 
    - `window.print()`
- **Document Object Model:** creates a model of the current webpage. 
    - `document.querySelectors('body')`
- **Global JavaScript Objects:** they are not an individual model but rather a group of objects that relate to different parts of the JavaScript language. 
    - `Math.random()`