+++
title = "Callback Function"
description = "This is an area for technical documentation"
weight = 2
+++

The **Callback function** creates a function inside the other function as a parameter. As it is showed in the example below, **checkInput** function has a **cb** callback function as a first parameter and **...strings** variable as a second rest parameter.
The callback function is called only when **hasEmptyText** condition is false, that means that there is no empty strings in the **...strings** variable. When **checkInput** function is called there is an array function **()=>** as a **cb** callback function in its parameters and several strings in the **...strings** variable. As there is no empty strings in the **...strings** variable, there will be 'All not empty' string printed into the console.

```
function checkInput(cb, ...strings){
  let hasEmptyText = false;
  for (const text of strings) {
    if (text === !text) {
      hasEmptyText = true;
      break;
    }
  }
  if(!hasEmptyText) {
    cb();
  }
}
checkInput(() => {
  console.log('All not empty');
},
'Hello',
'34',
'adfgetayufdgr',
'something'
);
```
