---
title: "Hackerrank - Weather Observation Station 17 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 17 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Weather Observation Station 17"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-17)

### Solution one:

```sql
select round(long_w,4) from station where lat_n > 38.7780 order by lat_n limit 1;
```
