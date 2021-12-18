---
title: "Hackerrank - African Cities solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-join']
date: 2021-07-04
lastmod: 2021-07-04
featured: false
draft: false
---
Problem [link](https://www.hackerrank.com/challenges/african-cities)

### Solution one:

```sql
select city.name from city left join country on city.countrycode = country.code where continent = 'africa';
```
