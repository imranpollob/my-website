---
title: "Hackerrank - African Cities solution"
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
Problem [link](https://www.hackerrank.com/challenges/african-cities)

### Solution one:

```sql
select city.name from city left join country on city.countrycode = country.code where continent = 'africa';
```
