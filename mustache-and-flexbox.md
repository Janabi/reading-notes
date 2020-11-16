# Mustache and Flexbox
## mustache.js
**Mustache** is a javascript templating that save a lot of codes with rendering data from JSON file.

## Flexbox
**Flexbox** is a grid layout which makes displaying HTML elements more flexible than other properties in term of simplicity and easy understand.

```
.container {
    display: flex;
    flex-direction: reverse-row;
    flex-wrap: no-wrap;
    justidy-content: center;
    align-items: center;
}
```
* **Display** which will be flex in the container or parent element.
* **flex-direction** which has a default value of row but definitly you can change it into column or reverse column and row. So this gives an an indication that how the items or children inside the container will lay out on cross or main.
* **flex-wrap** which indicate the items of the container will keep on the same horizental axes.
* **justify-content** which mean that how the alignment of the items will be horizentally for row direction, or vertically for column direction.
* **align-items** which mean that how the alignment of the items will be vertically for row direction, or horizentally for column direction.

***The following code will define the main properties of items on that flex container will be and how they work***
```
.item {
    flex-grow: 2;
    flex-shrink: 2;
    flex-basis: 50px;
    /* flex: 2 2 50px; */
}
```

* **flex-grow** means that certain item will be much wider than the others.
* **flex-shrink** means that certain item will shrink it size rather than the rest.
* **flex-basis** means the default size of the item whether width or height.
* **flex** means a shorthand property for all the previous properties consecutively (grow shrink basis) of the items, not the container.