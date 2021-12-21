---
title: "Hackerrank - Weather Observation Station 10 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 10 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-select']
date: 2021-06-01
lastmod: 2021-06-01
featured: false
draft: false
linktitle: "Weather Observation Station 10"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-10)

### Solution one:

```sql
SELECT DISTINCT CITY FROM STATION WHERE  CITY REGEXP "[^AEIOU]$"
```
