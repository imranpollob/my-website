---
title: "Hackerrank - Top Competitors solution"
subtitle: ""
summary: "Hackerrank - Top Competitors solution. Most of the solutions are written in Python and Javascript, when possible multiple solutions are added."
authors: []
tags: []
categories: ['hackerrank', 'sql', 'basic-join']
date: 2021-07-04
lastmod: 2021-07-04
featured: false
draft: false
linktitle: "Top Competitors"
type: book
---
Problem [link](https://www.hackerrank.com/challenges/full-score)

### Solution one:

```sql
SELECT h.hacker_id,
       h.NAME
FROM   submissions s
       LEFT JOIN hackers h
              ON s.hacker_id = h.hacker_id
       LEFT JOIN challenges c
              ON s.challenge_id = c.challenge_id
       LEFT JOIN difficulty d
              ON c.difficulty_level = d.difficulty_level
WHERE  s.score = d.score
GROUP  BY h.hacker_id
HAVING( Count(*) > 1 )
ORDER  BY Count(*) DESC,
          s.hacker_id;
```
