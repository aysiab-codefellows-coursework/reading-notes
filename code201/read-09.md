# Class 09: Reading Assignment 09
*Sections read:*
- Ch. 7, Ch. 14 (HTML&CSS)
- CH. 6 (JavaScript&JQuery)

### Passwords Do Not Match: An Article on Events

When you create an account on a webpage, it will prompt you to make a password and retype it. Have you ever finished retyping the password, and then get a message saying then don't match! Me too! 

Websites make such a big *event* over it. 

They literally do.

"Events trigger scripts"; events are what give JavaScript the ability to make your webpage interactive with your user. When events are 'fired off' or raised, scripts get triggered. Select the element node that are going to respond to the event. Next, indicate or bind the event to the selected node. State the code you want to run when the event occurs; usually this is a function of some type. 

For example, when you scroll off the website element of retyping your password that triggers the event, the event then calls for the script to run, and the script is what gives you the error message. 

There are three ways of event binding, however the last one is considered outdated and bad practice. 
1. Traditional DOM Event Handlers
```
function passwordsMatch () {
    // code for checking if passwords match
}

var element = document.getElementById('password2');
element.onmouseout = passwordsMatch();
```
2. DOM Level 2 Event Listeners
```
function passwordsMatch() {
    // code for checking if passwords match
}

var element = document.getElementById('password2');
element.addEventListener('mouseout',passwordsMatch,false);
```
3. HTML Event Handlers

