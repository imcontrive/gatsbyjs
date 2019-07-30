---
title: Fundamental Concepts of ReactJS
date: "2019-07-30 T23:46:37.121Z"
---
### Fundamental Concepts of ReactJS
In this article, I hope to explain what I consider some of the most important fundamental React concepts you need to understand.
([Medium Link](https://medium.com/@psubham94/fundamental-a2e34ddb73e4))


## There are some topics will be discuss here.
1. What is React and Why Should We Use it ?
2. What is Declarative Programming ?
3. What is Imperative Programming ?
4. Declarative Programming vs Imperative Programming ?
5. What is JSX, Element and Component in React ?
6. What are the different types of Components In React ?
7. What is render in Props ?
8. Pure functions vs Impure functions ?
9. What is Reconciliation Algorithm ?
10. Why React is More Efficient ?

### Ready ??

# 1. What is React and Why Should we used it?
`ReactJS` is a open-source javaScript Library that was created by Facebook which is used for building user interfaces and handling view layer for web and mobile apps. It’s also allow to create reusable UI components.

The core objective of ReactJS is providing the best possible rendering performance. The reason behind using ReactJS is to be fast and scalable and simple. It allows us to create large web applications which can change data, without reloading the page.

## Why Should We Used ReactJS ?
There are so many open-source javaScript frameworks for making the front-end web application easier, like Angular , Ember, Vue. Let us to take a quick look on the benefits of Recat over other frameworks.

### Simplicity :
 `ReactJS` uses plain JavaScript and its lifecycle is clearly defined. It is easy to use the component-based approach to build your website or mobile application.

 ### Easy to learn :
 Anyone with a basic previous knowledge in programming can easily understand React. For React just need basic knowledge of CSS , HTML and JavaScript.

 Native Approach : React can be used to create mobile applications (React Native). React is a diehard fan of reusability, meaning extensive code reusability is supported.
Data Binding : In React, there’s no two-way data-binding.It uses one-way data binding and an application architecture called Flux controls the flow of data to components through one control point — the dispatcher. It’s easier to debug self-contained components of large ReactJS apps.
Performance: React just updates the essential part of the DOM being updated. React does not offer any concept of a built-in container for dependency.
Testability : ReactJS applications are super easy to test. React views can be treated as functions of the state, so we can manipulate with state we pass to the ReactJS view and take a look at the output and triggered actions, events, functions, etc.
2. What is Declarative Programming ?
Declarative programming is a programming paradigm in which the programmer defines what needs to be accomplished by the program without defining how it needs to be implemented.
In other words, the approach focuses on what needs to be achieved instead of instructing how to achieve it.
3. What is Imperative Programming ?
Imperative programming is a programming paradigm in which the programmer defines how to accomplish the program without defining what needs to be accomplished by the program.
Imperative programming describes a sequence of steps that change the state of the computer. Imperative programming explicitly tells the computer “how” to accomplish it.
4. Declarative Programming vs Imperative Programming ?
Declarative programming :
i) What to do ?
ii) A style of building the Structure and elements of the computer programs.
iii) It expresses the logic of a computation whithout describing it’s control.
Imperative programming :
i) How to do ?
ii) It’s a programming paradigms that uses the statements that change a Program’s state.
iii) It’s describes the control for the computations or for changing the state of Programs.
5. What is JSX, Element and Component in React ?
JSX :
i) JSX is a preprocessor step that adds XML syntax to JavaScript.
ii) JSX is a XML-like syntax extension to ECMAScript without any defined semantics.
iii) In other words, JSX is a syntax extension to javaScript. It produced react components.
const element = <h1> Welcome to ALtCampus </h1>
Element :
An element is a plain object describing a component instance or DOM node and It’s desired Properties.
Component:
i) It’s a basic building block of any React app.
ii) It is a javaScript class or function that optionally accepts input i.e. props and returns a React element that describes how a section of UI should appear.
6. What are the different types of Components In React ?
There are two types of components in ReactJS
i) Functional component :
Functional components are those components i.e. usually defined as a function of its state and props .
import React from 'react';

function App() {
  const greeting = 'Hello Function Component!';

  return <h1>{greeting}</h1>;
}

export default App;
ii) class component:
class components have some additional features .
class classComponent extends React.Component {
  render() {
     return <div> My Class Component </div> 
  }
}
7.What is render in Props ?
The term “render prop” refers to a technique for sharing code between React components using a prop whose value is a function.
<Provider render={data => (
  <h1>Hello {data.target}</h1>
)}/>
8. Pure functions vs Impure functions ?
Pure functions :
i) Pure functions are those functions that accept an input and returns a values without modifying any data outside it’s scope.
ii) A Pure function always returns the same value as the given input.
iii) A Pure function should not have any side effetcs like mutataing the data , console.log, Math.random and Rendering API calls.
Impure functions :
i) Impure functions are those functions that accept an input and returns a modifying data outside of it’s lexical scope.
ii) Impure functions mutates the variable /state /data outside of it’s lexical scope.
Lexical Scope : A convention used in many programs to sets the scope (range of functionality) of a variable so that it may only be called from within the code is defined.
In simple , lexical Scope means the variables defined inside a function .
9. What is Reconciliation Algorithm ?
i) In simple, “ Reconciliation is the action of making one view or belief compatible with another.”
ii) It’s a process through which react updates the DOM. When a components state’s changes ,React has to calculate if it is necessary to update the DOM. It does by creating a VIRTUAL DOM and comparing with the current DOM.
Virtual DOM :
‘“ The virtual DOM is the instance of existing DOM, that contain the new state of the component. ”’
10. Why React is More Efficient ?
React is more efficient because of Reconciliation (Diffing Algorithm). React re-render only that elements whose state are changed instead of overall element or view.
Hope you have enjoyed this article. In the next article, we will discuss the component life cycles of ReactJS. So, stay tuned for the next article.