---
title: "Hackerrank - The PADS solution"
subtitle: ""
summary: "Hackerrank - The PADS solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'advanced-select']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "The PADS"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/the-pads)

### Solution one:

```sql
SELECT CONCAT(NAME,'(',LEFT(OCCUPATION,1),')')
FROM OCCUPATIONS
ORDER BY NAME;
```

### Solution two:

```sql
SELECT CONCAT("There are total ",COUNT(OCCUPATION)," ",LOWER(OCCUPATION),"s.")
FROM OCCUPATIONS
GROUP BY OCCUPATION
ORDER BY COUNT(OCCUPATION),
         OCCUPATION;
```
