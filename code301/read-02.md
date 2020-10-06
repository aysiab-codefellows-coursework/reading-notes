# Reading Assignment Two
*Sections Read:*
- pgs. 293 - 301, 306-331, 354-357 (JS&JQuery)

### JQuery Basics Quiz
1. What goes in between the paranthesis when using JQuery: `$('your answer')`
2. ***TRUE OR FALSE*** JQuery is it's own language. 
3. What are Duckett's 3 main reasons for using JQuery?
4. Can JQuery objects be stored in variables? If yes, how? If no, why not?
5. ***TRUE OR FALSE*** .text() will return the string value of an element. 
6. ***TRUE OR FALSE*** JQuery objects can store multiple element references. 
7. What is the proper way to change a list item cucumber to birds in the given html?
```
<ul>
<li>Cats</li>
<li>Dogs</li>
<li>Cucumber</li>
</ul>
```
8. ***TRUE OR FALSE*** `.prepend()` & `.before()` are interchangable. 
9. What is the syntax for event handling in JQuery?
10. Where is the ideal location to place your JQuery script element in your HTML?

<hr/>

1. A CSS selector 
2. False
3. Simple Selectors, Common Tasks in Less Code, Corss Broswers Copatibility 
4. Yes, and the proper syntax is $variableName to differentiate from other JavaScript variables
5. True 
6. True
7. `$('li:contains('cucumber')').text('fish');`
8. False
9. `$('selector').on(event, function () {});`
10. Before the closing `</body>` tag
