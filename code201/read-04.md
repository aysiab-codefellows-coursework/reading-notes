# Class 04: Reading Assisgnment 04
*Sections read:*
- Ch. 4 Ch. 15 (HTML&CSS)
- Ch. 3 (JavaScript&JQuery)
- [This Article](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

### HTML Links
Links are important to web pages because they let you navigate among pages. Links are made up of the `<a href=""></a>` tags. 

Basic structure of a link:

`<a href="https://github.com/">Github</a>`

Result:

<a href="https://github.com/">Github</a>

Links can take you to internal pages, external pages, page elements, and mail-to. You can also add the attribute `target`and set it to `target = "_blank"` to open in a new window. 

### CSS Layouts Basic
When considering layouts, it is innmportant to remember that elements are all boxes to CSS. Block elements are the main building blocks for your CSS layout. 

Block level elements can sit inside other block level elements. The outer box elements are considered container elements. 

CSS has several positioning schemes for your elements:
1. Normal Flow
    - the default behavior where every block element will sit vertically underneath each other. Even if there is enough width for multiple elements side by side, they will still sit on top of another in normal flow. 
2. Relative Positioning
    - relative positioning will move an element either down, right, left relative to where it would sit in normal flow. 
3. Absolute Positioning
    - elements are positioned in relation to their containing element; they are taken from normal flow and do not affect surrounding elements. Absolute positioning means the elements will move as you scroll. 
4. Fixed Positioning
    - Fixed positioning is a type of absolute positioning, but instead of the element being in relation to the containing element, the relation is to the browser window. 
5. Floating Elements
    - floating elements can be moved to be positioned to the left or right of other elements, and are taken out of normal flow. However surrounding elements can flow around floated elements. 

    It is also important to consider the screen sizes of your users when making your layouts. You want your layouts to remain cohesive among all screen sizes and resolutions. 

    Also, you can use multiple style sheets for your webpages to keep things clean. For example, you can have a style sheet just for layout and different one that indicates color to your page. 

<hr />
    
### Functions

**Functions:** are a series of statements (tasks) that you want to execute to perform a specific task. 

**Methods:** are essentially functions that take place within an object. 

To declare a new function:
```
function nameGoesHere(parameters) {
    /// something happens
    /// return value
}
```
Parameters are values that you need to pass into a function in order for your function to execute, you function can intake numerous parameters and they are separated by commas. Not all functions need parameters. 

Functions often return something after being called. They can return a single value or use an array to return several. 

To call a function:
```
nameGoesHere(parameter);
```
When it comes to functions, it is important to consider *variable scope*. Variable scope affects how you use and access variables within your code. 

For instance, a variable that is declared within a function can only be accessed within that function. This is known as local scope or function-level scope. 