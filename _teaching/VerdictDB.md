---
title: "VerdictDB"
collection: teaching
permalink: /experience/verdictdb
venue: "University of Michigan, EECS"
date: 2018-05-01
location: "Ann Arbor, US"
---

VerdictDB is the project I currently working on. It is a client-side library that speed up SQL queries greatly without any changes on original database by sacrificing a little accuracy.
&nbsp;

Starting from adding unit test for VerdictDB, I gradually become familiar with the inner logic of VerdictDB. During the summer of 2018, I have assisted finishing the task of reconstructing the whole project. I was first responsible for creating parser for the user input SQL query.
By using [Antlr](https://github.com/antlr/antlr4), the syntax tree has been created and SQL queries can be parsed into objects that VerdictDB can handle, which also includes some query standardization work that changes the structure of query.
&nbsp;

After that, I moved onto the modules that work as the backend of the program. The basic idea of VerdictDB is creating scrambling tables of huge tables, which makes partition for the original table. By doing so, VerdictDB issues query and gets answer
only from one part of huge table in order to speed up the querying. To achieve that, a tree-like query planning structure was created by us so that it can decompose a single query into separate nodes that perform different tasks. Besides implementing those nodes, one of the most important node is the node that performs aggregation function such as count(), avg() of big tables. To take the advantage of scrambling, I adopted the [producer and consumer model](https://en.wikipedia.org/wiki/Producer%E2%80%93consumer_problem) to
support the multi-thread processing.
&nbsp;

Meanwhile, I have also worked on creating JDBC interface of user level. By creating JDBC driver for VerdictDB and modifying syntax, VerdictDB now can support almost every database.
![alt text][logo]

[logo]: https://camo.githubusercontent.com/7500f5d36ab5320e4e026bf9b916cb170d38569b/687474703a2f2f7665726469637464622e6f72672f696d6167652f766572646963742d666f722d696d70616c612d737065656475702e706e67 "Performance of VerdictDB"
