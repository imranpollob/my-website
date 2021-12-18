---
title: "Hackerrank - Japan Population solution"
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
Problem [link](https://www.hackerrank.com/challenges/japan-population)

### Solution one:

```sql
SELECT SUM(POPULATION) FROM CITY WHERE COUNTRYCODE = "JPN";
```
