---
title: "Hackerrank - Population Density Difference solution"
subtitle: ""
summary: "Hackerrank - Population Density Difference solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Population Density Difference"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/population-density-difference)

### Solution one:

```sql
SELECT MAX(POPULATION) - MIN(POPULATION) FROM CITY;
```
