---
title: "Hackerrank - Weather Observation Station 13 solution"
subtitle: ""
summary: "Hackerrank - Weather Observation Station 13 solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Weather Observation Station 13"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-13)

### Solution one:

```sql
select round(sum(lat_n),4) from station where lat_n > 38.7880 and lat_n < 137.2345;
```
