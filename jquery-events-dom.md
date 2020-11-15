# jQuery - Events and the DOM

**-jQuery- is a JavaScript library that makes a shorthand for some javascript methods and functions especially those related to the animating, styling and making your website more dynamic.**

## How to start with jQuery?

See the follwoing block of code...
```
$(document).ready(function(){
    $('any html element').action();
});
```

The above block of codes indicate the folowing observations:
> $ (Dollar Sign) refers that you are enterend the origin jQuery file that contains all of its comomands.
> The docuemnt refers to the Html document that we are dealing with.
> The ready mans once the document is completely loaded then execute the following function.
> Then you also pick any html element and apply a certain jQuery buildup actions.

***Fortunately, they made a shorthand for the ready action in the following code:***
```
$(function(){
    // your jQuery code
});
```
***Also, you can choose any elements by their classes or IDs or even descendant elements***

# DOM on jQuery
## What does DOM mean?
**-DOM- mean -Document Object Model-**
As we known, these objects declared like a tree with its nodes, then for example, image that the html element is the tree and its child nodes are head and body elements and what elements go inside one of these child nodes, we will consider them as grandchild and so on.
***That's exactly DOM means to be!***:wink:

**To search for more jquery DOM traversal methods that are mainly used them to change somethig at any HTML element, see this -[LINK]-(https://www.w3schools.com/jquery/jquery_traversing.asp)**

# Events in jQuery
**Events are maily used in jQuery in order to do an action (e.g.click, hover over, press a key on keyboard, etc..). These will make certain changes in html or css layout.**

lets take a couple of code examples 
```
$('.btn').click(function(){
    $('p.answer').show();
});
```
\*To understand what going to happen in the previous code:
* First, we decide to make the action as a click on a button that has a class called btn.
* Secondly, this event will show (show is an action) the answer for that question (a paragraph element with class 'answer')


