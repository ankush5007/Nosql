Ques 1- What are the top reasons to choose Nosql?
Ans 1
=====
Reference
---------
https://www.geeksforgeeks.org/top-5-reasons-to-choose-nosql/?ref=rp
https://www.thoughtworks.com/insights/blog/nosql-databases-overview






Ques 2 - What is the main difference between Mongodb vs DynamoDb ?
Ans 2
======
Reference
---------
https://www.xplenty.com/blog/dynamodb-vs-mongodb-differences/#:~:text=DynamoDB%20is%20a%20fully%20managed,fully%20managed%20with%20MongoDB%20Atlas.&text=DynamoDB%20uses%20tables%2C%20items%20and,and%20has%20fewer%20size%20restrictions.




Ques 3 - Types of NoSQL Databases Explain ?
or
Ques 3 - What and When to use Nosql Explain ?
Ans 3
=====
Reference
---------
https://www.educative.io/courses/definitive-guide-to-mongodb/7DjJ35jO4Dj?aid=5082902844932096&utm_source=google&utm_medium=cpc&utm_campaign=dynamic2&gclid=Cj0KCQiArvX_BRCyARIsAKsnTxNsHz0hWQNz8GpledOFRe2juRhHW_nDGFR8Sl6MF2b_2se4VoKnco4aApJNEALw_wcB
https://www.guru99.com/nosql-tutorial.html#:~:text=NoSQL%20Database%20is%20a%20non,and%20real%2Dtime%20web%20apps.
https://www.analyticsvidhya.com/blog/2020/09/different-nosql-databases-every-data-scientist-must-know/
https://www.mongodb.com/nosql-explained
https://www.digitalocean.com/community/tutorials/a-comparison-of-nosql-database-management-systems-and-models

- NoSql scales horizentally and distrubuted in nature beucase these are no relational database

-There are four type of Nosql database category 
- Key Value store
- Document store
- Colum Family
- Graph base Store





Ques 4 - Explain Nosql Database Architectural Comparison ?
Ans 4
======
Reference
---------
https://griddb.net/en/docs/NoSQL_Database_Architectural_Comparison.pdf




Ques 5 - What are the key points to Consider while Picking Nosql database for storage Explain?
Ans 5
=====
Reference
----------
https://www.dataversity.net/choose-right-nosql-database-application/#


- There are many Types of Nosql database but few points always keep in mind
1 - What kind of data you want to store either as a document based or column based or graph based or key value based
2 - Nosql Database Distrubuted architecture
3 - Where This fits as of Cap Theorm
4 - Nosql use case




Ques 6 - What is Cap therom  Explain?
or
Ques 6 - What is the CAP Theorem? MongoDB vs Cassandra vs RDBMS, where do they stand in the CAP theorem?
or
Ques 6 - What are the characterstics of Distrubuted Theorm Explain?
Ans 6
=====
Reference
---------
https://bikas-katwal.medium.com/mongodb-vs-cassandra-vs-rdbms-where-do-they-stand-in-the-cap-theorem-1bae779a7a15
https://www.analyticsvidhya.com/blog/2020/08/a-beginners-guide-to-cap-theorem-for-data-engineering/
https://www.educative.io/edpresso/what-is-the-cap-theorem?aid=5082902844932096&utm_source=google&utm_medium=cpc&utm_campaign=edpresso-dynamic&gclid=Cj0KCQiA88X_BRDUARIsACVMYD8pNxFclqJofg6gdQtER2kMmqqfgHAoMXhJOwhzQ-GXdbnfcN50GigaAvAoEALw_wcB
https://www.analyticsvidhya.com/blog/2020/08/a-beginners-guide-to-cap-theorem-for-data-engineering/
https://medium.com/@bikas.katwal10/mongodb-vs-cassandra-vs-rdbms-where-do-they-stand-in-the-cap-theorem-1bae779a7a15
https://cloudxlab.com/assessment/displayslide/345/nosql-cap-theorem#:~:text=Partition%20Tolerance%20is%20a%20guarantee,the%20system%20continues%20to%20perform.
https://stackoverflow.com/questions/12346326/cap-theorem-availability-and-partition-tolerance
https://towardsdatascience.com/cap-theorem-and-distributed-database-management-systems-5c2be977950e
https://dzone.com/articles/understanding-the-cap-theorem
https://mwhittaker.github.io/blog/an_illustrated_proof_of_the_cap_theorem/
https://www.ibm.com/cloud/learn/cap-theorem#:~:text=A%20partition%20is%20a%20communications,between%20nodes%20in%20the%20system.

Cap therom
===========
- Cap stands for Consistent , Availbilty and Parition Tolerence To understand this let understand the distrubuted system.DS are the network where data are stored more than one machine or nodes(virtual or physical) at a same time and serving will be done at the same time. all cloud Application now a days are distrubuted system.

- Any distrubuted can not deliver all three characterstics of CAP therom at a time

- Consistent ,Availabilty and Parition Tolerence are the characterstics while designing distrubuted system.cap theorm tells that a distrubuted system can not deliver all three characterstics at a same time any of two can be applied at same time.Every RDBMS or Nosql has it's own Characterstics (CAP) either they support CA or CP or AP  so accordingly you can pick database and work accordingly.
- Generally To build a distrubuted system we prefer mostly nosql datanase becuase they have default horizental scaling distrubuted architecture where we can put more machines or node to scale fast and to elimnate single point of failure

- Consistent Means Data will be in Consistent state every time means all client will see the same data at same time there will be no inconsistent state.no matter in which node they connect and request query for read or write should gets up to date data. if client make a write request that updated data on one node should be replicated to all other nodes on the spot before acknowledging back to the client so if another clients make read request it should get updated data connected from any node in the cluster.so in Consistent system if one data writes value in one node it should expect to get the fresh value from any node 
- Availablity means data should be available request should be served by a node as a response if one of the nodes are down other nodes are responsible to deilver response
- Partition Tolerence  is a comminication break with in distrubuted system.or communicatio break down between two or more nodes.So means Cluster should continue to work despite any break down between the node
- Today, NoSQL databases are classified based on the two CAP characteristics they support:All Nosql Comes under this

- CA Database
=============
- RDBMS(Mysql,Sql Server) support two characterstics of CAP theorm at a time in distrubuted system
- A CA database delivers consistency and availability across all nodes. It can’t do this if there is a partition between any two nodes in the system, however, and therefore can’t deliver fault tolerance. system will go down

- CP Database
==============
- Mongodb ,Hbase,Redis support two characterstics of CAP theorm at a time in distrubuted system
- A CP Based Database Provided consistency and Parition Tolernce at the expense of Availabilty means if Partition Occure between two nodes so system has to shut down the in consistent node to maintain the consistency for other nodes and make it unavailable until partition is resolved.so technically availablity is not given pr provided

-AP Databse
============
- Cassandra ,Couch Db,Riak,DynamoDb support two characterstics of CAP theorm at a time in distrubuted system
- AP Database provide Availbilty and Partition tolorence at the expense of Consistency . means if any partition occurs between Nodes so nodes should be available and provide wrong unconsistent data but will not get down.when ever Partition resolves then AP databse typically resync fresh data with other nodes to repair all inconsistency in the system.




Ques 7 - Difference between Sharded Nothing and Shared disk Architecture Explain?
or
Ques 7 - Shared Nothing Architecture: The Key to Scale Your App to Millions of Users Explain?
or
Ques 7 - Why Old based typical file system can not scaled as horizental scaling Explain ?
Ans 7
=====
Reference
---------
https://www.geeksforgeeks.org/difference-between-shared-nothing-architecture-and-shared-disk-architecture/
https://mobisoftinfotech.com/resources/mguide/shared-nothing-architecture-the-key-to-scale-your-app-to-millions-of-users/
http://www.benstopford.com/2009/11/24/understanding-the-shared-nothing-architecture/




Ques 8 - What is Graph Database and Use case Explain ?
or
Ques 8 - How Do You Know If a Graph Database Solves the Problem?
or
Ques 8 - What are the real UseCase to pick Graph Database over other Nosql database ?
or
Ques 8 - How social media Plateform use Graph Database efficently Explain?
or
Ques 8 - How Google Map use Graph Database Effiecently Explain?
Ans 8
======
Reference
---------
https://www.profium.com/en/blog/graph-database-use-cases/
https://medium.com/neo4j/how-do-you-know-if-a-graph-database-solves-the-problem-a7da10393f5
https://medium.com/@6point6ltd/use-cases-for-graph-databases-37ceb4903edd
https://www.bmc.com/blogs/graph-database-use-cases/
https://neo4j.com/use-cases/
https://www.profium.com/en/blog/graph-database-use-cases/
https://neo4j.com/blog/native-vs-non-native-graph-technology/
https://neo4j.com/developer-blog/how-do-you-know-if-a-graph-database-solves-the-problem/
https://medium.com/@ja3606/using-facebook-to-learn-some-basics-about-graph-theory-ecadb31cd127
https://medium.com/dev-genius/graph-database-vs-relational-database-70f6156f7415
https://medium.com/@mtbuzzerseo/graph-database-vs-relational-database-e5798281f6ef
https://www.youtube.com/watch?v=UodTzseLh04
https://neo4j.com/developer/graph-db-vs-rdbms/
https://www.profium.com/en/blog/graph-database-use-cases/#:~:text=The%20Graph%20Database%20is%20optimized,such%20as%20GDPR%20and%20HIPAA.
https://neo4j.com/blog/5-noteworthy-use-cases-graph-technology-analytics/
