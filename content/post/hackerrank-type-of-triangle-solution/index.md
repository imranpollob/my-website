---
title: "Hackerrank - Type Of Triangle solution"
subtitle: ""
summary: " "
authors: []
tags: []
categories: ['hackerrank', 'sql', 'advanced-select']
date: 2021-05-01
lastmod: 2021-05-01
featured: false
draft: false
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
