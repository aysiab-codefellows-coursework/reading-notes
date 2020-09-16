# Class 13: Reading Assignment 13
*Sections Read:*
- [Article](http://diveinto.html5doctor.com/storage.html)

### Local Storage
HTML5 offers a unique solution to a local storage issue that has long been a problem for webpages. Cookies have been available for a long time but can't store much data without slowing down the runtime of your webpage. 

Local storage is an object that stores data in key: value pairs. Local storage takes thing in as strings *only* and therefore a work around is needed to store arrays and objects. For that we use `JSON.stringify()`.

Let's start with creating a new object to store in our local storage. 

```
var Pet = function (name,age,species) {
    this.name = name;
    this.age = age;
    this.species = species;
}

var iggy = new Pet('Iggy',2, 'dog');

```
Now that we have our object  `iggy` made let's store it. We use `localStorage.setItem()` to create a new key:value pair.

```
localStore.setItem('Iggy',JSON.stringify(iggy));
```
To retrieve our object from local storage, we also need to convert it back to an Object. We would call use `localStorage.getItem()` to retrieve our object by using the key we assigned. 
```
localStorage.getItem(JSON.parse('iggy'));
```
`JSON.parse()` is how we are able to turn our object string back into an object. 

If we want to delete the single object we would use `localStorage.removeItem('key')`, and to delete all of our local storage we would use `localStorage.clear()`.