---
title: "Hackerrank - The Blunder solution"
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
Problem [link](https://www.hackerrank.com/challenges/the-blunder)

### Solution one:

```sql
SELECT CEIL(AVG(SALARY)-AVG(REPLACE(SALARY, 0 , ''))) FROM EMPLOYEES;
```
