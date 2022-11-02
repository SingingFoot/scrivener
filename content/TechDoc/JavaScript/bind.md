+++
title = "Function.prototype.bind()"
description = "This is an area for technical documentation"
weight = 1
+++

The **bind()** method creates a new function that, when called, has its **this** keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.


```
const person1 = {
    name: 'Oleh',
    age: 46,
    logInfo: function() {
        console.log(`Name is ${this.name}`);
        console.log(`Age is ${this.age}`);
    }
};

const person2 = {
    name: "Svitlana",
    age: 37
};

person1.logInfo();
person1.logInfo.bind(person2)();
```
As a result of using the method **bind()**, it is possible to borrow the **logInfo** function of **person1** object to the **person2** object. 

```
Name is Oleh
Age is 46
Name is Svitlana
Age is 37
```

This way, the function of the first object **person1** is called in the context of the second object **person2**, which saves many lines of code that no longer need to be added to the second object. This is especially important if the function of the first object is very complex or repeated many times for a large number of different objects.

Methods **call** and **apply** are very similar to **bind** in the sense of the context, but they don't need to be called like **bind** `person1.logInfo.bind(person2)();`. 

```
person1.logInfo.call(person2);
person1.logInfo.apply(person2);
```

Panyi Szabolcs
1113 Budapest
Bocskai út 43. VI. lph 3. em/132
Phone: 36304652636
For Svitlana Shynkarenko

Username: singingfoot@gmail.com
Your new Password: M1IFH18Z
www.escadaviragkuldes.hu

