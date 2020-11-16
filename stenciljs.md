---
date: 2020-11-16T00:17
---


# StencilJS

Web Component creation system.

A Web Component is defined using TypeScipt and is then compiled into
a propert web-standards Web Component.

```
import  { Component, Prop, h } from  '@stencil/core';

@Component({
  tag: 'my-component',
  styleUrl: 'my-component.css',
  shadow: true
})

export  class  MyRatingComponent  {
 @Prop() maxValue: number = 5;
 @Prop() value: number = 0;

 createStarList() {
   let starList = [];

   for (let i = 1; i <= this.maxValue; i++) {
     if (i <= this.value) {
       starList.push(<span class="rating">&#x2605;</span>);
     } else {
       starList.push(<span class="rating" >&#x2606;</span>);
     }
   }

   return starList;
 }

  render() {
   return  (
     <div>
       {this.createStarList()}
     </div>
   );
  }
}
```


### stenciljs
