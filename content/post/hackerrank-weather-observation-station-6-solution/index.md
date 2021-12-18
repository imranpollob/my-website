---
title: "Hackerrank - Weather Observation Station 6 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-6)

### Solution one:

```sql
SELECT DISTINCT CITY FROM STATION WHERE CITY LIKE "A%" OR CITY LIKE "E%" OR CITY LIKE "I%" OR CITY LIKE "O%" OR CITY LIKE "U%";
```

### Solution two:

```sql
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[AEIOU]';
```
