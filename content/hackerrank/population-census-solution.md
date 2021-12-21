---
title: "Hackerrank - Population Census solution"
subtitle: ""
summary: "Hackerrank - Population Census solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-join']
date: 2021-07-04
lastmod: 2021-07-04
featured: false
draft: false
linktitle: "Population Census"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/asian-population)

### Solution one:

```sql
select sum(city.population) from city left join country on city.countrycode = country.code where continent = 'asia';
```
