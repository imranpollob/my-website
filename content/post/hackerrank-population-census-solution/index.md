---
title: "Hackerrank - Population Census solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-join']
date: 2021-07-04T15:17:25+06:00
lastmod: 2021-07-04T15:17:25+06:00
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/asian-population)

### Solution one:

```sql
select sum(city.population) from city left join country on city.countrycode = country.code where continent = 'asia';
```
