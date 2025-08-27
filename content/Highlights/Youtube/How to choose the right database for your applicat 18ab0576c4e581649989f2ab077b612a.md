---
draft: true
description:
socialDescription:
title: How to choose the right database for your applicat 18ab0576c4e581649989f2ab077b612a
date: 2025-03-05
modified: 2025-08-21
---
# How to choose the right database for your application - Zoe Steinkamp - NDC Oslo 2023

Created time: January 29, 2025 9:04 AM
Finished: No
Link: https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo
Status: To Learn
Tags: NDC Conferences
Total Videos: 1
Video Duration: 00:41:02

### [0:00 Intro](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=0s)

### [1:12 Some Database History](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=72s)

SQL is initially developed at IBM

1980’s - SQL becomes the standard lang for relational databases

![image.png](image%2013%202.png)

graphDB makes social media

time series is for iot devices

![image.png](image%2014%202.png)

![image.png](image%2015%202.png)

![image.png](image%2016%202.png)

![image.png](image%2017%202.png)

### [8:49 Primary Index Data Structure](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=529s)

![image.png](image%2018%202.png)

![image.png](image%2019%202.png)

### [11:56 Hot and Cold Storage](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=716s)

![image.png](image%2020%202.png)

### [13:25 Durability and Disaster Recovery](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=805s)

![image.png](image%2021%202.png)

### [14:43 Building Our Own Company](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=883s)

### [15:13 Building the Foundation](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=913s)

### [17:10 Scaling and Personalization](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1030s)

### [21:05 Fast and Efficient Search](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1265s)

![image.png](image%2022%202.png)

Most people in web use elastic search

### [23:49 Enhanced Performance](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1429s)

### [25:57 One Example of Redis in Use](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1557s)

![image.png](image%2023%202.png)

![image.png](image%2024%202.png)

### [26:53 Real-Time Insights - Time Series](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1613s)

![image.png](image%2025%202.png)

![image.png](image%2026%202.png)

### [29:16 Analyzing and Monitoring - Time Series](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1756s)

### [30:09 Data organization](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=1809s)

![image.png](image%2027%202.png)

### [35:42 Visual Search Revolution](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=2142s)

### [37:19 Vector DB's Visauls](https://www.youtube.com/watch?v=hj2yFugmpz8&type=snipo&t=2239s)

Comments:

For over 99% of companies PostgreSQL and the extensions available are FOSS and can do anything they need. Relational, document, vector, timeseries, graph, KV, etc. Postgres has you covered. Want row store, compressed row store, column format storage or even parquet storage? Postgres has that covered. Want scaleout? Postgres has that covered too. It’s all free and you can deploy it anywhere. If you want to start with something start there. If you then realise that you need something that is a little bit better because it is very specialised then change. However, I cannot think of anything where there is an order of magnitude difference between Postgres + extensions and more specialised publically available DB that more than at most 1% of companies might need.