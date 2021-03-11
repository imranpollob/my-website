---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Avoid chain variable assignments in JavaScript"
subtitle: ""
summary: "Chaining variable assignments may seem fancy but have unintended consequences associated with it."
authors: []
tags: []
categories: ["javascript"]
date: 2021-03-11T14:21:55+06:00
lastmod: 2021-03-11T14:21:55+06:00
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

Chaining variable assignments may seem fancy but have unintended consequences associated with it. During chaining of variable assignments, implicit global variables are created which results in polluting the global namespace.

```javascript
// bad
(function example() {
  let x = (y = z = 1);
  // JavaScript interprets this as
  // let x = ( y = ( z = 1 ) );
  // The let keyword only applies to variable x, variables y and z become
  // global variables and thus polluting global namespace.
})();

console.log(x); // throws ReferenceError
console.log(y); // 1
console.log(y); // 1

// good
(function example() {
  let x = 1;
  let y = x;
  let z = y;
})();

console.log(x); // throws ReferenceError
console.log(y); // throws ReferenceError
console.log(z); // throws ReferenceError
```
