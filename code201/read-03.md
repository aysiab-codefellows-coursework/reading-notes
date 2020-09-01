# Class 03: Reading Assisgnment 03
*Sections read:*
- Ch. 3 Ch. 13 (HTML&CSS)
- Review Ch. 2, Ch. 4 (JavaScript&JQuery)

### HTML Lists
In HTML you can have unordered lists, ordered lists, and definition lists. You can also nest lists inside of lists!

**Unordered List:** `<ul></ul>`

**Ordered List:** `<ol></ol>`

*Your list items need to be within `<li></li>` tags nested within the `<ul> or '<ol>` tags*

**Definition Lists** are constructed using `<dl><dl>` with `<dt></dt>` tags nested inside for the defined term, and then `<dd></dd>` for the definition

### CSS Boxes
As previously stated, CSS treats every HTML element as it's own box. These boxes have padding, borders and margins that can be manipulated to dictate size, and alignment in relation to each other. 

Additionally, these boxes can change visibility, enable scrollbars, broder images and even box shadows. 

<hr/>

### JavaScript Loops

***For loops:***

```
for(var i = 0; i < 25; i++) {
    // do something here
}
```

In order for a for loop to work there are 3 steps to be taken. 
1. Initialization 
    - this is the `var i = 0;` within the for loop
2. Conditional
    - the conditional states for how long the loop will keep repeating the process
    - in this case the conditional is `i < 25;`
3. Update
    - the update will update our variable until the condition is met
    - `i++` is the update

Our example loop will run 25 times. 

***While Loops***
```
var x = 0;

while (x != 5) {
    console.log(x);
    x++;
}
```

In order for a while loop to work, the variable(s) must be initialized outside of the loop conditional. The loop will stop after the conditional is no longer valid. 

*Do while* loops are similar except that the code will run at least once before checking the conditional to continue looping. 

```
var x = 0; 

do {
    console.log(x)
    x++;
} while(x != 5);
```

**Important**

`break` is an important keyword that you can use in your loops to break out of the loop

`continue` is another important keyword that you can use in your loops, it tells the interpretor to stop the current iteration, update and check the condition again. If the condition is met, the loop continues. (Duckett, pg 174)

Infinite Loops occur when the conditional in the loop never reaches a `false` condition. This means your loops will keep going on infinitely. 