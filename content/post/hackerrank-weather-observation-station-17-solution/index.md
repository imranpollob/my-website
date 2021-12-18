---
title: "Hackerrank - Weather Observation Station 17 solution"
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
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-17)

### Solution one:

```sql
select round(long_w,4) from station where lat_n > 38.7780 order by lat_n limit 1;
```
