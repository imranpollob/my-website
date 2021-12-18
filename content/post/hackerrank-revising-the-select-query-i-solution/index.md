---
title: "Hackerrank - Revising the Select Query I solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-select']
date: 2021-06-01T15:17:25+06:00
lastmod: 2021-06-01T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/revising-the-select-query)

### Solution one:

```sql
SELECT * FROM CITY WHERE COUNTRYCODE = "USA" AND POPULATION > 100000;
```
