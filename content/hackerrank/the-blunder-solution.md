---
title: "Hackerrank - The Blunder solution"
subtitle: ""
summary: "Hackerrank - The Blunder solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "The Blunder"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/the-blunder)

### Solution one:

```sql
SELECT CEIL(AVG(SALARY)-AVG(REPLACE(SALARY, 0 , ''))) FROM EMPLOYEES;
```
