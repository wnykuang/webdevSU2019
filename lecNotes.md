# Lec Note - May 8  

## Relationship of resources and servers

Browers -> Servers: HTMLs, CSS files back to Browser.
Parse by the browser, DOM.  
Some of the reference will not ask for the severs but for the cloud, like bootstrap. Like some kind of CDN.  
First download the HTML, and get the CSS file.  
The browser keeps the cache of the files.  
The sequence to get resouces:

1. check the cache.(Maybe you have already get the resouces from other websites.)
2. ask the resource online.  

## BootStrap

### INSTALLING BOOTSTRAP

Download ZIP  
CDN

### CONTAINER CLASSES

### GRID SYSTEM

Pages look better when laid out in columns. Early in WWW history it was common to misuse TABLEs. Use DIVs and CLASSes instead to achieve same behaviour.  
12 columns: easy to break up with 3\4\6. Ideas from publication industry.  
"md" in class, "medium" size col. "col-md-4" 4 columns for medium screens and larger screen. (will only triggle when the screen is medium.)
"xs" will be only triggled when the screen is extra small or larger.  
"container" is only for the outmost wrapper.  

### BREAK POINTS

Based on px. Can check out the detail infomation on the Bootstrap 3's document.  

IDE: WebStorm  
Should use bootstrap lib to styling. (It's using the bootstrap 4.)
form-control class get the better layout.  
Using the grid system to control the layout.  
Two main roles to layout:  

1. Inline behaviour. One word after another word. "Text" inside.  
2. Behaviour of the block, entire the page. Full behaviour of the "div".

By default, the input field behaviour inline.  With the css, we can overwrite the behaviour. From inline to block.

## What is JavaScript

JS is the programming language of the Web. Can be embadded into the webpage.

```html
<script>
    alert("hello");
</script>
```

However, it's a bad practise to write it inline to html, should be seperated with another js file.
Js is a popular server side programming language as well.
JS manipulating the DOM, render the page.  
Can put breakpoint in the js and css in chrome.  
It's pretty low-level.  
JS objects, syntax referred to as JSON or JavaScript Object Notation.  

### Use strict

Enforce some best practices by configuring strict language validation.  

### IIFE

Inmediatedly Invoked Fuction Expression
There is no package in js, will have name collosion. Will be overwriten by newer function. In the current version of the JS, we have namespacing problem. Inside function is indeed local, will be not overwritten. To declare the namespace. In the function is only living inside function.  
Put everything into a function. Could ensure everything run but not be overwritten.  

## JQuery
jQuery is a JS library that simplifies JS development. jQuery abstracts the browers to deal with fragmentation.  

### Syntax
jQuery defines a global function called jQuery and its alias $.  

```javascript
$(selector).action(parameter);

$("p").css("color", "red");
//Hide elements with class="details"
$(".detail").hide()
```

Put the code in the end of the body. Then could ensure all the elements have been loaded.(in raw JS)
jQuery can subscribe to onload event to wait for browser to build the DOM.

```javascript
$(document).ready(function(){
    // jQuery/js code to operate on DOM
})
```
Js does not support overload but jQuery support.