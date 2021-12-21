---
title: "Hackerrank - Weather Observation Station 2 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 2 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Weather Observation Station 2"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-2)

### Solution one:

```sql
select round(sum(lat_n),2), round(sum(long_w),2) from station;
```
