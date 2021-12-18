---
title: "Hackerrank - Revising Aggregations - The Count Function solution"
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
Problem [link](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function)

### Solution one:

```sql
SELECT COUNT(ID) FROM CITY WHERE POPULATION > 100000;
```
