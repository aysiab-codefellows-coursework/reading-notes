# Reading Assignment Thirteen
*Read:*
- [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

# Sending Form Data Summary
First of all let's refresh how forms are structured in html.They begin with a `<form></form>` tag. 

`<form>` tags can have an `action` attribute. The action attribute defines where the data from the form gets sent via either a valid relative path (`/this/directory`) or an absolute URL (`https://mywebsite.com`)

If no `action` attribute is specified, the data gets sent to the page the form resides. 

Another attribute that can be added to forms is the `method` attribute. The `method` attribute can only be assigned to `GET` or `POST` method. 

The `GET` method is used when the browser is asking the server to send back a specific resource. Whereas, the `POST` method is different in the way that it talks to the server; in the case of a form, it would append the form data to the body of the request. The request would then take a look at the body and send back the corresponding result. 

There are many server side languages such as Perl, Java, .Net, & Ruby but it's more common to use a framework such as Express for Node.js if working with JavaScript like we are in this class. 

Security is something that needs to be greatly considered whens ending data back to your server. 