# Responsive Web Design and Floats

## What does the resposive web design mean?
**It is a method to build up an entire which can be fit and resposive into any different devices or the screen sizings**

### Responsive Web Design breaks down into thre components:
- Flexible Layout
- Media Queries
- Flexible Media

## Flexible Layout
**The idea of using a -relative units- (e.g.%, em, vh, wh, vmin, vmax) rather than -fixed units- (e.g.inch or pixel)**
**Relative units are depending on the width and height of the device or screen**

## Media Queries
### Media queries are mainly based on two categories:
1. The viewport of the specified device or screen.
2. The orientation of the web page.

***Highly preferable to use max- or min- in width or height at the media query features.*** :ok_hand:
The default of the media type is 'screen'.

***Don't also forget to use \*Respond.js\* to make the media query woking perfectly on IE8 or below this version.***

\*In order to take the width and height of the browser
> Don't forget to use the **Viewport meta tag** in your HTML head tag.

### Last notes about RWD
- max-width property makes the media elements (e.g.Photos, videos, others) more scalable.
- However, iframe tag doesn't work for max-width, therefore, it's better to position it absolutely to its relative parents.

# Floats
**One of earliest way to make the block elements stacked together horizentally.**

**Don't forget to use the clear method in order to keep the following elements in its original position.**

### Powerful methods to clear the following elements from the floated one
- make an empty div after the floated elements.
- assign an overflow property of the parent element into hidden.
- using the significant easy clear method which is identified into the following blocks of codes:

'''
.clearfix::after {
    content: "";
    clear: both;
    display: table;
}
'''

