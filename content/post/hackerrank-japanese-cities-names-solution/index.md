---
title: "Hackerrank - Japanese Cities Names solution"
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
Problem [link](https://www.hackerrank.com/challenges/japanese-cities-name)

### Solution one:

```sql
SELECT NAME FROM CITY WHERE COUNTRYCODE = "JPN";
```