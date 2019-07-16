---
title: JavaScript object creation Patterns
date: "2015-07-14T22:12:03.284Z"
---
In this article we will learn about various different ways to create objects in
JavaScript like Object Literal,Factory Pattern, Constructor Pattern, Prototype 
Pattern, Dynamic Prototype Pattern.([Medium Link](https://medium.com/@psubham94/the-ultimate-guide-to-understanding-local-storage-2a27fdb80544))

<!-- Oh, and here's a great quote from this Wikipedia on
[salted duck eggs](http://en.wikipedia.org/wiki/Salted_duck_egg). -->

If you are learning JavaScript, you must have come across the term Object.
In JavaScript ,Everything is an object. An object is an entity having state and 
behavior (properties and method). Properties are the values associated with a 
JavaScript object and methods are actions that can be performed on objects.


> JavaScript Object creation by object literal

This is the simplest way to create an object. In which key value pairs are sep
-arated by ':' inside a set of curly braces({ }) like below:
``` js
  var student = {
    
  subject : "JavaScript" ,
    
  mentor : "ankit"
    
  };
```

> JavaScript Object creation by Factory Pattern

A factory is a function or method that returns objects of a varying prototype or
class from some method call. Any  function which is not a class or constructor 
that returns a new object ,those functions are Factory Function.

```js
  function userCreator(name, score){
    const user = Object.create(userMethods);
    user.name = name ;
    user.score= score ;
    return user;
  }
  var userMethods = {
    sayName :function() {
      this.name ;
    },
    incrementScore: function(){
      this.score++ ;
    }
  }
  var user1 = userCreator("ankit",95);
  //{name: "ankit", score: 95}
```

will be completed soon....