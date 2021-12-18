---
title: "Hackerrank - Weather Observation Station 16 solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'aggregation']
date: 2021-05-01T15:17:25+06:00
lastmod: 2021-05-01T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/weather-observation-station-16)

### Solution one:

```sql
select round(lat_n,4) from station where lat_n > 38.7780 order by lat_n limit 1;
```
