# Reading Assignment Three
*Sections Read:*
- [Flexbox Article](https://flexboxfroggy.com/)
- [Flexbox Froggy](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Mustache.JS Article](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

### Flexbox Basics:
Flexbox are CSS properites that are designed to make templating and creating layouts with a 'flexible box'. Flexbox has CSS properties for both container/parent elements as well and individual child elements. 

Before you can get started with using Flexbox, you must define the display as flex within the CSS rules for your containing element

```
main {
    display: flex;
}
```
The container element actually has multiple different properties that can be used. 

```
main {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-evenly; 
    align-content: flex-end;
}

```

`flex-direction` dictates how your containing element's children are oriented. Either horizontally in a row, or vertically in a column. Both values can be reversed.

`flex-wrap` dictates how the children are aligned in the containing element; the wrap value indicates that additional elements should wrap to the next available space in the containing element. For our code example above, for all intents and purposes a new row of children elements would be created due to the `wrap` value.

`justify-content` dictates how the children elements are aligned horizontally. However, this becomes vertical alignment if the value for `flex-direction` is reversed. 

`align-content` acts similarly to `justify-content` except it's innate behavior is to align vertically. Again, it becomes horizontal alignment instead if the `flex-direction` is reversed. 

Additionally, `flex-flow` is shorthand for `flex-direction` and `flex-wrap`

Now, children elements can have their individual Flexbox properites:

```
#candy {
    order: 1;
    flex-grow: 2;
    flex-basis: 1;
    align-self: flex-end;
}
```
`order` can move individual elements around to change how they are displayed. Negative numbers moving the element over to the left, and positive numbers moving the element over to the right. Every number accounts for the number of elements the element you are targeting is moving over. 

`flex-grow` accepts a unitless value as a proportion for the given element to grow to. 

`flex-shrink` is essentially the inverse of `flex-grow`

`flex-basis` defines the default size of the element before any remaining space is distributed. 

`flex` is shorthand (and the reccommended convention) for `flex-grow` `flex-shrink` and `flex-basis` combined. 

`align-self` this allows for the default alignment given by the parent container to be overwritten for individual flex items. 