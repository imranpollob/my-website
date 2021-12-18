---
title: "Hackerrank - Population Density Difference solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/population-density-difference)

### Solution one:

```sql
SELECT MAX(POPULATION) - MIN(POPULATION) FROM CITY;
```
