---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Reverse a string in various programming language"
subtitle: ""
summary: "Reversing is a common task in programming. Different language handle this task differently."
authors: []
tags: ["javascript", "php", "python"]
categories: ["javascript", "php", "python"]
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

Reversing is a common task in programming. Different language handle this task differently. I will try to figure it out in one place.

PHP:

```
$a = "Hello World!!!";
echo strrev($a);
```

Python:

```
a= "Hello World!!!"
print(a[::-1])
```

JavaScript:

```
var word = "Hello World!!!";
console.log(word.split("").reverse().join(""));
```
