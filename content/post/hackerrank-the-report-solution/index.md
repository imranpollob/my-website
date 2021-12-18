---
title: "Hackerrank - The report solution"
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
Problem [link](https://www.hackerrank.com/challenges/the-report)

### Solution one:

```sql
SELECT CASE
           WHEN g.grade<8 THEN NULL
           ELSE s.name
       END,
       g.grade,
       s.marks
FROM students s
JOIN grades g ON s.marks BETWEEN g.min_mark AND g.max_mark
ORDER BY g.grade DESC,
         s.name,
         s.marks;
```
