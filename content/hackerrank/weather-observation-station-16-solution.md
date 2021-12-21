---
title: "Hackerrank - Weather Observation Station 16 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 16 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Weather Observation Station 16"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-16)

### Solution one:

```sql
select round(lat_n,4) from station where lat_n > 38.7780 order by lat_n limit 1;
```
