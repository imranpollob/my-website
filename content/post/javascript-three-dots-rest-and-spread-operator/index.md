---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Javascript Three Dots Rest and Spread Operator"
subtitle: ""
summary: "Javascript three dots (...) to handle array, object and string."
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

I like to learn by example. I think you too. Let's tackle Rest and Spread operator.

- You can expand an array, an object or a string using the spread operator (...). Let's start with an array example. Given

```js
const a = [1, 2, 3];
```

- You can create a new array using

```js
const b = [...a, 4, 5, 6];
```

- You can also create a copy of an array using

```js
const c = [...a];
```

- This works for objects as well. Clone an object with:

```js
const newObj = { ...oldObj };
```

- Using strings, the spread operator creates an array with each char in the string:

```js
const hey = "hey";
const hiArray = [...hey]; // ['h', 'e', 'y']
```

- This operator has some pretty useful applications. The most important one is the ability to use an array as function argument (**spread element**) in a very simple way.

```js
const fun = (foo, bar) => {};
const a = [1, 2];
fun(...a);
Math.max(...a); // 3
```

(in the past you could do this using f.apply(null, a) but that's not as nice and readable)

- The **rest element** is useful when working with **array destructuring**.

```js
const numbers = [1, 2, 3, 4, 5]
[first, second, ...others] = numbers
```

- ES2018 introduces **rest properties**, which are the same but for **object destructuring**.

```js
const { first, second, ...others } = {
  first: 1,
  second: 2,
  third: 3,
  fourth: 4,
  fifth: 5,
};
first; // 1
second; // 2
others; // { third: 3, fourth: 4, fifth: 5 }
```

- ES2018 has **spread properties** allow to create a new object by combining the properties of the object
  passed after the spread operator.

```js
const items = { first, second, ...others };
items; //{ first: 1, second: 2, third: 3, fourth: 4, fifth: 5 }
```

- There is also a special array-like object named `arguments` that contains all arguments by their index. When rest parameters did not exist in the language, and using arguments was the only way to get all arguments of the function.

```js
function show() {
  console.log(arguments.length); // 4
}

show(1, 2, 3, 4);
```

Notes:

- Arrow function doesn't have own `arguments`, it takes them from the outer “normal” function.
- When ... is at the end of function parameters, it’s “rest parameters” and gathers the rest of the list of arguments into an array.
- When ... occurs in a function call or alike, it’s called a “spread operator” and expands an array into a list.
