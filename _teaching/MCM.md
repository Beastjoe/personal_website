---
title: "The Mathematical Contest in Modeling 2018"
collection: teaching
permalink: /experience/mcm
venue: "University of Michigan, EECS"
date: 2018-02-01
location: "Ann Arbor, US"
---

The Mathematical Contest in Modeling 2018(MCM 2018) is a good experience to practice applying data gathering and analyzing skill for me.
&nbsp;
&nbsp;


The topic our group chose was Problem B: estimating the population of every languages in the future.
One of the most difficult problem is how to get data of the population of every language in the past. Although it's easy to google which are the most
popular languages, it is hard to get the specific population data of those language, especially when we want to investigate the language that is not
very popular. The solution I come up is to check the history of wiki. Every month, wiki updates the population of language, so a python script using BS4 was
created to automatically gathering data from wiki tables.
&nbsp;

After gathering the data, we took the analytic hierarchy process to combine the factors that may decide the trend of language population. Using this method, we
predicated how population of languages will change in next 50 years. Also, based on the pattern of migration, we also give a predication on the geographical distribution of languages.
Finally, we have receive Meritorious Winner for our paper.
&nbsp;

![alt text](/images/pop.png "pop")
&nbsp;
Figure 1. Predicted Population of Language

![alt text](/images/migration.png "migration")
&nbsp;
Figure 2. Migration Pattern of Population of Language

