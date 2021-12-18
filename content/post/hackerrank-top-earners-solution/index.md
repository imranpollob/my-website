---
title: "Hackerrank - Top Earners solution"
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
Problem [link](https://www.hackerrank.com/challenges/earnings-of-employees)

### Solution one:

```sql
select months*salary as e,count(*) from employee group by e order by e desc limit 1;
```
