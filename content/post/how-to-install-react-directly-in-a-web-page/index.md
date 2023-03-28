---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "How to install React directly in a web page"
subtitle: ""
summary: "We can add React JS file directly to web page without using create-react-app"
authors: []
tags: ["react"]
categories: ["react"]
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

We can add React JS file directly to web page without using `create-react-app`. We have to include a couple of files to achieve our goal.

- react.production.min.js (main react file).

- react-dom.production.min.js (talk with dom).

- babel.min.js (to run JSX).

- own js file with "text/babel" mime type.

index.html

```html
  <body>
    <div id="root"</div>

    <script src="https://unpkg.com/react@16/umd/react.production.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.production.js" crossorigin></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>

    <script src="script.js" type="text/babel"></script>
  </body>
```

script.js

```js
const Button = () => {
  return <button>Click me!</button>;
};

ReactDOM.render(<Button />, document.getElementById("root"));
```
