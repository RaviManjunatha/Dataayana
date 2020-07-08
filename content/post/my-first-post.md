---
title: "Cloud Datawarehouse : The Big Shift"
date: 2020-06-29T14:26:45+05:30
draft: false
image: 'BigShift.png'
---

Interviews for BI Engineers usually comprised of questions from SQL, Star & Snowflake schema design, different chart types that he /she will use to develop a report, the challenges encountered in the project and questions on the toolset used. I very rarely came across interviewers who would quiz on the  data compression techniques,sizing, backup, disaster recovery, latency, migration & deployment scenarios. The popular notion was that it was generally left to the 'Infra team' or the 'Enterprise Architect'  or the 'DBAs' to deliberate on these.

A typical datawarehouse implementation involved Data Analysts, ETL Developers, Data Modellers,DBAs,Testers and Data Architects. Design principles generally involved  denormalizing the OLTP to a OLAP system, workflow management, alerts & notifications. 

The emphasis on compressing the data, writing efficient queries, workload management was less and since the initial VMs came with all high configurations, the performance was always blazing initially.

Fast forward to the mid life of the Datawarehouse, tickets on Jobs failing due to disk space issues, out of memory errors, reports not refreshing due to long queues were the norms. I  was tasked with  the upkeep of one such datawarehouse built on a Learning Management Application for an Oil& Gas major. My days used to start with the dreaded ETL jobs which behaved erratically as the VMs had reached their hardware limits. Owing to the increase in the number of incidents , based on the root causes identified, i recommended vertical scaling of the VM with few of the ETL queries re-written and using materialized views.

It was taken up as en enhancement project and took nearly a months' time to get all the approvals to scale the VMs. The other changes took another 2 months for completion.

It worked , but i knew that it was a band-aid solution and the problems would re surface at some point in time.

Fast forward to the times of Cloud Datawarehouse, i was working as a Solution Architect for implementing a Data warehouse solution for Gold mining company. It was my first tryst with Redshift and i was literally blown away by the multi dimensional capabilities that it came with.

The initial pitch for Redshift was that it was a 'SQL' like cloud data warehouse solution and that any SQL developer could easily learn and start working on it from day-1. 

As i started exploring more on Redshift and its powerful features, i realized the learning curve of Redshift for a SQL developer is quite steep.

Let me eulogise this a bit more, as it is cloud native, it comes with enhanced agility, elasticity and no-ops requirements. One can easily alter the nodes and its types and see the changes in performance in a matter of hours.

It gives developers the options to compress data, look for efficient sort mechanisms, think of workload management for efficient handling of queues and much more. While the traditional RDBMS had some of these options, Redshift simplifies these concepts and the developer docs come to the rescue of a any newbie developer who is curious to learn & implement.

A couple of Redshift developers can now accomplish what a team of Data Analysts, ETL Developers, DBAs & Architects could do.

The feature that i am particularly impressed is its pricing mechanism. Since it is based on pay on usage , it puts a great premium on writing in-efficient queries. Many a times in the on-prem Data warehouses we are left with many used tables, queries and reports. Yet we continue to house them and dont audit their usage. Cloud Datwarehouses like Redshift puts a premium on such archaic data items. 

Small enterprises  who erstwhile would have  struggled with the development cost of implementing a blazing datawarehouse on-prem, can now leverage the cloud datawarehouse which abstracts the complexity of the massively parallel scalable datawarehouse development. Given the volatility that surrounds a budding enterprise, cloud datawarehouse like Redshift offers the perfect solution.

GDPR, Data security concerns are often cited as drawbacks of cloud databases and datawarehouses. Redshift comes with region based availability and has encryption options, i personally feel enterprises should embrace cloud datawarehouses for non-critical applications to start off and cite the design of Redshift to ask their solution architects to come with such design in their on-premise datawrehouses where possible.

The Big shift in the datawarehouse world has taken place, it is time for data professionals to include cloud datawarehouses like Redshift in their learning to-dos and carry out pocs in their organisations and influence the decision makers to embrace this shift.

