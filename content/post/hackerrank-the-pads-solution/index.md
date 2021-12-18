---
title: "Hackerrank - The PADS solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'advanced-select']
date: 2021-05-01T15:17:25+06:00
lastmod: 2021-05-01T15:17:25+06:00
featured: false
draft: false
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
