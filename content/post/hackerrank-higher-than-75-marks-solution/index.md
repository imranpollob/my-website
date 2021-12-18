---
title: "Hackerrank - Higher Than 75 Marks solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-select']
date: 2021-06-01
lastmod: 2021-06-01
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/more-than-75-marks)

### Solution one:

```sql
SELECT NAME FROM STUDENTS WHERE MARKS > 75 ORDER BY RIGHT(NAME,3),ID;
```
