---
title: "Hackerrank - Weather Observation Station 4 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-4)

### Solution one:

```sql
SELECT COUNT(CITY) - COUNT(DISTINCT CITY) FROM STATION;
```
