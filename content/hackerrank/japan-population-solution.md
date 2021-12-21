---
title: "Hackerrank - Japan Population solution"
subtitle: ""
summary: "Hackerrank - Japan Population solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Japan Population"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/japan-population)

### Solution one:

```sql
SELECT SUM(POPULATION) FROM CITY WHERE COUNTRYCODE = "JPN";
```
