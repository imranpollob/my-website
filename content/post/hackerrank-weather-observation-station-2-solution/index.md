---
title: "Hackerrank - Weather Observation Station 2 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-2)

### Solution one:

```sql
select round(sum(lat_n),2), round(sum(long_w),2) from station;
```
