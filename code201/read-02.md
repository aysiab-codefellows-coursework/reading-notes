# Class 02: Reading Assisgnment 02
*Sections read:*
- Ch. 2, Ch. 10 (HTML&CSS)
- Ch. 2, Ch. 4 (JavaScript&JQuery)

### HTML Text Tags

| Tag        | HTML Example                                | Result                                     | Element Type |
|------------|---------------------------------------------|--------------------------------------------|--------------|
| `<h1>`     | `<h1>Heading</h1>`                          | <h1>Heading</h1>                           | Block        |
| `<p>`      | `<p>Paragraph</p>`                          | <p>Paragraph</p>                           | Block        |
| `<sup>`    | `Example<sup>superscript</sup>`             | Example<sup>superscript</sup>              | In line      |
| `<sub>`    | `Example<sub>subscript</sub>`               | Example<sub>subscript</sub>                | In line      |
| `<strong>` | `<strong>Strong<strong>`                    | <strong>Strong</strong>                    | In line      |
| `<em>`     | `<em>Emphasis</em>`                         | <em>Emphasis</em>                          | In line      |
| `<ins>`    | `Cats are <del>awesome</del> <ins>rude</ins>` | Cats are <del>awesome</del> <ins>rude</ins>  | In line      |
| `<del>`    | `Cats are <del>awesome</del> <ins>rude</ins>` | Cats are <del>awesome</del> <ins>rude</ins> | In line      |
| `<s>`      | `I love cats <s>and dogs</s>`               | I love cats <s>and dogs</s>                | In line      |


*`<h1>` is the biggest and foremost heading option, however there are options in descending size importance down to `<h6>`

HTML elements are used to define the basic structure of the webpage but can also contain semantic information. 
<hr/>

### CSS Basics

Consider every HTML element is individually wrapped up as a present. CSS can individually wrap these presents and make them appear differently on the outside in terms of color, alignment, and font. 

CSS can either be *external* or *internal* to your HTML. 
- Extermal CSS uses the `<link>` tag
    - `<link bref ="style.css">`
- Internal CSS uses the `<style>` tag
    -`<style>CSS GOES DIRECTLY HERE</style>`

*Regardless, both of these tags should be within your `<head>` tag in your HTML file. Remember, your `<head>` tag will hold all your meta data and mechanics.*

CSS has a series of *selectors* that are used to define style for certain areas of your webpage. 

***Three Basic Selectors***

**Type Selectors**
- they match element names
    - h1 {}
    - p {}

**Class Selectors**
- they match elements' class attribute
- class attributes can be applied to more than one element
    - if your html is `<p class="note">` then the CSS selector would be .note{}

**ID Selectors**
- they match elements' id attribute
- id attributes can only be individually applied to an element
    - if your html is `<h1 id="title">` then the CSS selector would be #title{}

There are also *child selectors, descendent selectors, adjacent sibling selectors, general sibling selectors*

CSS is made up of selectors that declare what element you are changing, and within every selector {} you will be defining a property and value.  A property is declaring what you are changing, and the value is how exactly you are changing it. 

For example, let's say you want to change your h1 elements to the color blue. You would use the type selector to say you want the changes to apply to h1{}. Then you would use the property `color` to declare that you are specifically changing the color, and you would add the value `blue`. 

*Example* 

h1 {

 color: blue;

}

**HOW CSS WORKS:** CSS is short for *Cascading Style Sheets*, and CSS rules due cascade and use inheritence. 
- If two selectors are identical then the latter of the two will take precedence. 
- If one selector is more specific than the other, the more specific rule will take precedence. 
    - However `!important` can be added to indicate that this propert value is more important


<hr />

### JavaScript Basic Syntax
JavaScript is an asynchronous programming language used to run scripts for web pages. Each individual instructrion or step is known as a statement, and every statement written needs to end with a semi-colon.

Each statement should also begin on a new line for clarity, and ease of reading your code. 

Your code should also contain commeents that explain what each bit of code is doing or what it should be doing. 
- Comments in JavaScript are started with //.  
- Multi line comments are written /* like this */ 

Data can be stored in variables. Using variables can cut down on the redundancy of your code and also make it easier to read. However, JavaScript is case sensitive so a variable named cubeHeight will be different than CUBEHEIGHT or CubeHeight. 

There are different data types that can be stored in variables. You can store numeric data types, string data types, and boolean data types. 

Example declarations:
- `var stringExample = "Hello world!";`
- `var numericExample = 5;`
- `var booleanExample = true;`
- `var nothingYet;` 
    - this variable will automatically be set to `null`

Arrays are a special type of variable; they can store multiple values. Arrays do not need you to specify how many values it needs to contain. 

Declaring an array:
- `var colors;`
- `colors = ["white","red","yellow"];`

To access values in an array, you need to use their index number. Arrays begin their index at 0. For example our array `colors` above would have have an index of 0-2. Let's say, I want to store my favorite color red in a new variable. It would look like this:
- `var faveColor = colors[1];`

JavaScript also makes use of arithmetic operators:
- `+` adds one value to another
- `-` subtracts one value to another
- `/` divides two values
- `*` multiplies two values
- `++` adds one to current value
- `--` subtracts one from current value
- `%` divides two values and returns the remainder

**Note**: Strings can also use the `+` operator to combine strings together, or strings and numbers. Numbers added to a string will automatically be converted to a string. 

**Basic Decision  Making:**
Conditionals are used for basic decision making. These comparisons between values will result either boolean; `true` or `false`. 
- `==`is equal to
- `!=` is not equal to
- `===` is strict equal to
- `!==` is strict not equal to
- `>` is greater than
- `<` is less than
- `>=` is greater than or equal to
- `<=` is less than or equal to

Logical Operators:
- `&&` logical AND
- `||` logical OR
- `!` logical NOT

Conditional and logical operators are often used within if/else statements. An if statement defines a conditional, and if the condition is met, the code within the if statement will run. Else is used to give alternate instructions to run. 

Switch statements assume a default to run, and have other instructions if the conditonal is met. 