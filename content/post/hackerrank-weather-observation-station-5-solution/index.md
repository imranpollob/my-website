---
title: "Hackerrank - Weather Observation Station 5 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-5)

### Solution one:

```sql
SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) DESC LIMIT 1;
```

### Solution two:

```sql
SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) LIMIT 1;
```
