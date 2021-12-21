---
title: "Hackerrank - Type Of Triangle solution"
subtitle: ""
summary: "Hackerrank - Type Of Triangle solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'advanced-select']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
linktitle: "Type Of Triangle"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/what-type-of-triangle)

### Solution one:

```sql
SELECT
  CASE
    WHEN A+B>C AND A+C>B AND B+C>A
      THEN
        CASE
          WHEN A=B AND B=C THEN "Equilateral"
          WHEN A=B OR B=C OR A=C THEN "Isosceles"
          ELSE "Scalene"
        END
      ELSE "Not A Triangle"
  END
FROM TRIANGLES;
```
