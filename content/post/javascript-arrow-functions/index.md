---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Javascript Arrow Functions"
subtitle: ""
summary: "Arrow function is the most significant change in ES6/ES2015 and since its introduction changed how JavaScript code looks and works."
authors: []
tags: ["javascript"]
categories: ["javascript"]
date: 2021-03-11
lastmod: 2021-03-11
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
highlight: true
---

Arrow function is the most significant change in ES6/ES2015 and since its introduction changed how JavaScript code looks (and works).

```js
const myFunction = function () {
  //...
};
// Arrow function
const myFunction = () => {
  //...
};
```

- If the function body contains just a single statement, you can omit the brackets and write all on a single line.

```js
const myFunction = () => doSomething();
```

- Parameters are passed in the parentheses.

```js
const myFunction = (param1, param2) => doSomething(param1, param2);
```

- If you have one (and just one) parameter, you could omit the parentheses completely.

```js
const myFunction = (param) => doSomething(param);
```

- For one-line statement in the function body, it will implicitly return without having to use the return keyword.

```js
const myFunction = () => "test";
myFunction(); //'test'
```

- When returning an object, remember to wrap the curly brackets in parentheses to avoid it being considered as function body brackets.

```js
const myFunction = () => ({ value: "test" });
myFunction(); //{value: 'test'}
```

- **Arrow functions do not have this. If `this` is accessed, it is taken from the outside.**

```js
const group = {
  title: "Our Group",
  students: \[("John", "Pete", "Alice")],

  showList() {
    this.students.forEach((student) =>
      console.log(this.title + ": " + student)
    );
  },
};

group.showList();
/*
"Our Group: John"
"Our Group: Pete"
"Our Group: Alice"
*/
```

Here in `forEach`, the arrow function is used, so `this.title` in it is exactly the same as in the outer method `showList`. That is: `group.title`.

```js
const group = {
  title: "Our Group",
  students: \[("John", "Pete", "Alice")],

  showList() {
    this.students.forEach(function (student) {
      // Error: Cannot read property 'title' of undefined
      console.log(this.title + ": " + student);
    });
  },
};

group.showList();
/*
"undefined: John"
"undefined: Pete"
"undefined: Alice"
*/
```

The error occurs because `forEach` runs functions with `this=undefined` by default, so the attempt to access undefined.title is made. That doesn’t affect arrow functions, because they just don’t have this.

- When defined as a method of an object, in a regular function `this` refers to the object, so you can do:

```js
const car = {
  model: "Fiesta",
  manufacturer: "Ford",
  fullName() {
    // same as fullName: function()
    return `${this.manufacturer} ${this.model}`;
  },
};

car.fullName(); // "Ford Fiesta"
```

- The `this` scope with arrow functions is inherited from the execution context. An arrow function does not bind this at all, so its value will be looked up in the call stack, so in this code `car.fullName()` will not work, and will return the string "undefined undefined"

```js
const car = {
  model: "Fiesta",
  manufacturer: "Ford",
  fullName: () => {
    return `${this.manufacturer} ${this.model}`;
  },
};

car.fullName(); // "undefined undefined"
```

**Due to this, arrow functions are not suited as object methods.**

- Arrow functions **cannot be used as constructors** either, when instantiating an object will raise a TypeError .
- **When dynamic context is not needed, use regular functions instead.** Example: when handling events, DOM Event listeners set `this` to be the target element, and if you rely on this in an event handler, a regular function is necessary:

```js
const link = document.querySelector('#link') link.addEventListener('click', () => {
// this === window
})
const link = document.querySelector('#link') link.addEventListener('click', function() {
// this === link
})
```
