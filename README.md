Element.Create.js
=================

This module creates element on the DOM using vanilla javascript;

Author: Wilfredo Pacheco

### CreateElement   
This method uses document.createElement to return an element based on the arguments passed.

Options is defined by the user to create a DOM element, below is an example of how to create an element:
``` javascript  
const LeftEl = CreateElement({
    tag: 'div',
    classList: 'row col px-2',
    parent: Widget,
})
.render();

/** Total Groups; */
CreateElement({
    tag: 'div',
    classList: 'p-3',
    parent: LeftEl,
    innerHTML: /*html*/`<!-- Total Groups -->
    <div>Total Groups</div>
    <div class="group-count" style="font-size: 2.5em; font-weight: 500;">${TotalGroups}</div>`
})
.render();
```


### CreateElementNode  
This method uses document.createElementNS to return an element based on the arguments passed.