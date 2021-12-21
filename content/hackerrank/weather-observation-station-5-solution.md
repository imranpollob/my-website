---
title: "Hackerrank - Weather Observation Station 5 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 5 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-select']
date: 2021-06-01
lastmod: 2021-06-01
featured: false
draft: false
linktitle: "Weather Observation Station 5"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-5)

### Solution one:

```sql
SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) DESC LIMIT 1;
```

### Solution two:

```sql
SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) LIMIT 1;
```
