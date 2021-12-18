---
title: "Hackerrank - Weather Observation Station 13 solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-13)

### Solution one:

```sql
select round(sum(lat_n),4) from station where lat_n > 38.7880 and lat_n < 137.2345;
```
