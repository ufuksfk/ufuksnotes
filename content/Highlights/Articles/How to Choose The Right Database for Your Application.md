---
draft: true
description:
socialDescription:
title: How to Choose The Right Database for Your Application
tags:
  - highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[GeeksforGeeks]]
url: https://www.geeksforgeeks.org/how-to-choose-the-right-database-for-your-application/

last highlighted date: [[2025-01#27]]
[[Database comparison and list]]
## Highlights
- • How much data do you expect to store when the application is mature?
  • How many users do you expect to handle simultaneously at peak load?
  • What [****availability****](https://www.geeksforgeeks.org/availability-in-system-design/), [****scalability****](https://www.geeksforgeeks.org/what-is-scalability-and-how-to-achieve-it-learn-system-design/), [****latency****](https://www.geeksforgeeks.org/what-is-latency/), ****throughput****, and ****data consistency**** does your application need?
  • How often will your [****database schemas****](https://www.geeksforgeeks.org/database-schemas/) change? [[Wiki/Others/Database schema]]
  • What is the geographic distribution of your user population?
  • What is the natural “shape” of your data?
  • Does your application need [****online transaction processing (OLTP)****](https://www.geeksforgeeks.org/on-line-transaction-processing-oltp-system-in-dbms/), [****analytic queries (OLAP)****](https://www.geeksforgeeks.org/olap-operations-in-dbms/), or both?
  • What ratio of reads to writes do you expect in production?
  • What are your preferred programming languages?
  • Do you have a budget? If so, will it cover licenses and support contracts?
  • How strict are you with invalid data being sent to your database? (Ideally, you are very strict and do server-side data validation before persisting it to your database)
- Another example is [[ArangoDB]] which has excellent performance but libraries for this ****DBMS**** are still young and lack support. Using ****ArangoDB**** in combination with other tools may be risky, so the community suggests avoiding ****ArangoDB**** for complex projects
- s it really going to grow unbounded over time? if so then you need some sort of ****database**** technology that is not limited to the data that you can store on one PC. You need to look at something like [[cassandra]] or [[mongoDB]] or [HBase](https://www.geeksforgeeks.org/architecture-of-hbase/) where you can actually distribute the storage of your data across an entire cluster and scale horizontally instead of vertically
- Many databases can’t handle thousands of users querying terabytes or petabytes of data, because of scaling issues.
- ****Databases**** with high ****throughput**** can support many simultaneous users. If we are talking about thousands then again a single ****database**** service is not going to work out.
- You will have to choose a ****database**** that is distributed and allows you to spread out a load of those transactions more evenly. In those situations, [[NoSQL]] [****NoSQL**** ****databases****](https://www.geeksforgeeks.org/introduction-to-nosql/) are a good choice instead of [****RDBMS****](https://www.geeksforgeeks.org/rdbms-full-form/) [[Relational database]]
- The truth is most of the [[NoSQL]] database we’ve talked about if you configure them with their default settings there will be ****no security**** at all.
- CAP stands for ****Consistency, Availability, and Partition tolerance****. The theorem states that you cannot achieve all the properties at the best level in a single database, as there are natural trade offs between the items. [[CAP theorem]]
	- You can only ****pick two out of three**** at a time and that totally depends on your prioritize based on your requirements. For example, if your system needs to be available and partition tolerant, then you must be willing to accept some latency in your consistency requirements. [[CAP theorem]]
	- ****Traditional relational databases**** are a natural fit for the ****CA**** side whereas ****Non-relational database**** engines mostly satisfy ****AP and CP**** requirements.
- ![CAP Consideration](https://media.geeksforgeeks.org/wp-content/uploads/20200824220237/CAPTheoremSystemDesign.png)
- ****Consistency**** means that any read request will return the most recent write. Data consistency is usually “strong” for SQL databases and for NoSQL database consistency may be anything from “eventual” to “strong”.
- ****Partition tolerance**** means the system will continue to operate despite network or node failures.
- ****Relational databases**** store data in a fixed and predefined structure. It means when you start development you will have to define your [****data**** ****schema****](https://www.geeksforgeeks.org/database-schemas/) in terms of tables and columns. You have to change the ****schema**** every time the ****requirements**** change. This will lead to creating new columns, defining new relations, reflecting the changes in your application, discussing with your ****database administrators****, etc
- the NoSQL database doesn’t put a restriction on the types of data you can store together. It allows you to add more new types as your needs change. In the application building process, most of the developers prefer high coding velocity and great agility.
- If you don’t need to deal with the massive ****scale**** then there is no need to use a ****NoSQL database****, you can choose ****MySQL**** and somewhere it’ll be fine.
