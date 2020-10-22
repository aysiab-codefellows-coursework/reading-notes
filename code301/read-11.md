# Reading Assignment Elevent
*Read:*
- [EJS Video Tutorial](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

### EJS *Embedded JavaScript templating*

EJS advertises on their site: using plain JavaScript, Fast Development time, Simple Syntax and Speedy Execution.

EJS is easily installed using NPM! You can run JavaScript within an .ejs file 

The syntax is simple! Typically only using `<% %>` as the base tags. 

Let's say we are sending some information over containing movie information, and we want to list all the movie titles. With EJS we could do something like:

```
<ul>
    <% movies.forEach(movie => { %>
        <li><%=movie.title%></li>
    <% })%>
</ul>
```

With EJS we are able to use the native JavaScript feature .forEach and loop through the data and print only the movie titles to an `<li>.` tag. 

In Reading Assignment 12, we talk about how to use EJS to further templating by making partials. Partials are resuable pieces of HTML called that can be used across many pages. 
