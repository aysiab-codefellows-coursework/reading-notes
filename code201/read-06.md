# Class 06: Reading Assignment 06
*Sections read:* 
- [This Article](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)
- Ch. 3, Ch. 5 (JavaScript&JQuery)

### The Problem Domain
The problem domain is the most challenging part of programming as the author, John Sonmez says:
> "As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it."

He later explains that sometimes if the problem domain is too big and ambigious, to try:

>"cutting out cases and narrowing your focus to a particular part of the problem."

### JavaScript Objects & DOM Quiz
1. Objects are a set of grouped together variables and functions that create a model for something. In objects, variables and functions are called:
    - a) Variables and functions 
    - b) Keys and values
    - c) Properties and methods 
    - d) Attributes and pairs 

2. ***Fill in the blank:*** objects can't have two of the same _______ names. 

3. ***True or False:*** the following code is the appropriate way to make an object using *literal notation*
```
var shop = new Object();
shop.name = "Nook's Cranny";
shop.type = "Convenience";
shop.inventory = ["Seeds","Shovel","Medicine"]; 
```

4. Which of the following ways can you update properties of an object?
    - a) `shop.name = "Able Sisters' Tailor"`
    - b) `shop["name"] = "Able Sisters' Tailor"`
    - c) all of the above
    - d) none of the above

5. ***True or False:*** functions can be used to create many similar objects. 

6. ***True or False:*** arrays are a type of object.

7. In 1-2 sentences explain what is DOM?

8. ***Fill in the blank:*** Storing DOM tree element location as __________ is known as ____________. 

9. Which of the following are ways to access a single node in the DOM tree?
    - a) `getElementById()`
    - b) `querySelector()`
    - c) `getElementByClassName()`
    - d) A&B
    - e) B&C
    - f) all of the above 

10. What is this code doing?
```
var fruit = document.getElementbyId('fruit');
```

<hr />

### Correct Answers
1. C
2. Key
3. False
4. C
5. True
6. True
7. DOM is the Document Object Model that is neither part of HTML or JavaScript. It is used to make a model of an HTML page and to access and change said page. 
8. variables, caching DOM queries 
9. D
10. The referenced location of the element ID'd 'fruit' is being stored as a variable fruit. 