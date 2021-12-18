---
title: "Hackerrank - Weather Observation Station 15 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-15)

### Solution one:

```sql
select round(long_w,4) from station where lat_n < 137.2345 order by lat_n desc limit 1;
```
