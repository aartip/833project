# The Development and Application of Hadoop and NoSQL Outline 

## Aarti Parupudi, Quan Kong, Wenbo Wang

### 1. Abstract

### 2. Introduction (Aarti)




### 3. Review of Related Work

#### 3.1 Review on Hadoop (Quan)

* [MapReduce: Simplified Data Processing on Large Clusters](https://www.usenix.org/legacy/publications/library/proceedings/osdi04/tech/full_papers/dean/dean_html/index.html) (Quan)
* [Understanding the Power of Hadoop as a Service](https://docs.google.com/file/d/0BwMVEMCs7KRNNWIyT3hiRXhLWms/edit) (Quan)
* [The Hadoop Distributed File System](https://docs.google.com/file/d/0B2_4GOBGjarzTkdLZDBNbVdYTXM/edit) (Quan)

---

* Big Data Challenges
	* pic

* What is Hadoop
	* A scalable, fault-tolerant distributed system for  data storage and processing.

* Components of Hadoop
	* pic

* HDFS

* MapReduce

* Why Hadoop
	* Scalability
		* scale out architecture
	* Hardware failure
		* multiple copies of data
	* Read/Write disk slow
		* multiple disks for parallel read
	* Merge data from different reads
		* MapReduce

* Disadvantages
	* not fit for small and real time data application
	* join multiple data are complex
	* not efficient for query



#### 3.2 Review on NoSQL (Mac)

* [NoSQL Databases: a step to databases scalability in web environment](https://docs.google.com/file/d/0B2_4GOBGjarzckFhYmxkODNkVUE/edit) (Mac)
* [NoSQL Databases](https://docs.google.com/file/d/0B2_4GOBGjarzaTdjcFhoODZVQWs/edit) (Mac)
* [A Comparison Between Several NoSQL Databases](https://docs.google.com/file/d/0B2_4GOBGjarzdnpWUk1GQjFndU0/edit?usp=drive_web) (Mac)

---

* Connections Between Papers
	* The first paper aims to focus on NoSQL databases in the context of cloud computing, talking about the origin and necessity of NoSQL movement. Then the second paper broadens the surface of study and introduces the details in NoSQL techniques, including the several data models and their applicable platforms. Then the third paper conducts a comparison between them and list their advantages and drawbacks. 


* **The Definition of NoSQL**: A NoSQL (often interpreted as Not Only SQL) database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.


* **A Little History**: The term NoSQL was first used in 1998 for a relational database that omitted the use of SQL. The term was picked up again in 2009 and used for conferences of advocates of non-relational databases. A blogger, often referred to as having made the term popular is Rackspace employee Eric Evans who later described the ambition of the NoSQL movement as “the whole point of seeking alternatives is that you need to solve a problem that relational databases are a bad fit for”. 


* **Motivation of NoSQL**: 
	* Avoidance of Unneeded Complexity;
	* High Throughput;
	* Horizontal Scalability and Running on Commodity Hardware;
	* Avoidance of Expensive Object-Relational Mapping;
	* Complexity and Cost of Setting up Database Clusters;
	* Compromising Reliability for Better Performance;
	* The current "One size fit's it all" Databases Thinking Was and Is Wrong;
	* The Myth of Effortless Distribution and Partitioning of Centralized Data Models;
	* Movements in Programming and Languages and Development Frameworks;
	* Requirements of Cloud Computing;
	* The RDBMS plus Caching-Layer Pattern/Workaround vs. Systems Built from Scratch with Scalability in Mind;
	* Yesterday's vs. Today's Needs;


* **Types of NoSQL databases**: this basic classification is based on data model. 
	* Column
	* Document
	* Key-value
	* Graph
	* Hybrid


* CAP-Theorem
	* **Consistency**: meaning if and how a system is in a consistent state after the execution of an operation. A distributed system is typically considered to be consistent if after an update operation of some writer all readers see his updates in some shared data source.
	* **Availability**: and especially high availability meaning that a system is designed and implemented in a way that allows it to continue operation (i.e. allowing read and write operations) if e.g. nodes in a cluster crash or some hardware or software parts are down due to upgrades.
	* **Partition Tolerance**: understood as the ability of the system to continue operation in the presence of network partitions. These occur if two or more “islands” of network nodes arise which (temporarily or permanently) cannot connect to each other. Some people also understand partition tolerance as the ability of a system to cope with the dynamic addition and removal of nodes.
	* CAP-Theorem - Alternatives, Traits, Examples<p><img src="Content/cap_theorem.png"/></p>
	* The CAP Theorem states, that for any system sharing data it is impossible to guarantee simultaneously all of these three properties. 
		* Particularly, in web applications based on horizontal scaling strategy it is necessary to decide between C and A. Usual DBMS prefer C over A and P. 

* ACID vs BASE
	* ACID
		* Atomicity
		* Consistency
		* Isolation
		* Durability
	* BASE
		* Basically Available
		* Soft-state
		* Eventual Consistency
	* <img src="Content/ACID_vs_BASE.png" alt="ACID vs BASE" />
	* BASE: an application work basically all the time (basically available), does not have to be consistent all the time (soft-state) but will be in some known-state state eventually (eventual consistency).

* Strict Consistency vs Eventual Consistency
	* Strict Consistency: according to Lipcon means that “All read operations must return data from the latest completed write operation, regardless of which replica the operations went to”. This implies that either read and write operations for a given dataset have to be executed on the same node2 or that strict consistency is assured by a distributed transaction protocol (like two-phase-commit or Paxos). As we have seen above, such a strict consistency cannot be achieved together with availability and partition tolerance according to the CAP-theorem.
	* Eventual Consistency: means that readers will see writes, as time goes on: “In a steady state, the system will eventually return the last written value”. Clients therefore may face an inconsistent state of data as updates are in progress. For instance, in a replicated database updates may go to one node which replicates the latest version to all other nodes that contain a replica of the modified dataset so that the replica nodes eventually will have the latest version.

* <img src="Content/data_models.png" />

* Sample NoSQL Databases: Apache Cassandra, MongoDB, Voldemort, Apache HBase, SimpleDB, BigTable, and OrientDB.

* NoSQL was designed to deal with massive data storage, but without working with a platform that support massive and parallel data processing, this technology is not fully utilized. 	

#### 3.3 Review on Hadoop + NoSQL (Aarti)

* [Integrating MapReduce and RDBMSs](https://docs.google.com/file/d/0B2_4GOBGjarzS09UbV8tTkR2ems/edit) (Aarti)
* [SQL-on-Hadoop Engines Explained](https://docs.google.com/file/d/0BwMVEMCs7KRNb1hici14RV9XVnc/edit) (Aarti)
* [Hadoop and NoSQL Technologies and the Oracle Database](https://docs.google.com/file/d/0BwMVEMCs7KRNUDJwaWx2Y2VyXzA/edit) (Aarti)
* [Optimizing Your Enterprise Architecture with Apache Hadoop and NoSQL](https://docs.google.com/file/d/0BwMVEMCs7KRNTjBCSzVQZ0E3OXc/edit) (Aarti)
* [Hbase: The Definitive Guide](https://docs.google.com/file/d/0B2_4GOBGjarzVXR3RUFwcXZxSzA/edit)

---

* Pros and Cons of Hadoop
	* Advantages
		* High data storage and processing scalability
		* Low price/performance ratio
		* High performance
		* High Availability
		* High schema flexibility
		* Capability to handle all types of data
		* Format free storage of data
	* Disadvantages
		* Hadoop API's like HBase, HDFS, MapReduce, are quite complex. They require expertise in Java Programming (or similar high-level languages) and require in-depth knowledge of how to parallelize query processing efficiently. 
		* The downsides of these interfaces are
			* a small target audience
			* low productivity
			* time consuming analysis
			* limited tool support

* What do we need??  
	What is needed is a programming interface that 
	* retains HDFS’s performance and scalability, 
	* offers high productivity and maintainability, 
	* is known to non-technical users, 
	* can be used by many reporting and analytical tools.  
	The obvious choice is - SQL!! 

* SQL is a 
	* high level, declarative and standardized database language
	* familiar to countless BI specialists, 
	* supported by almost all reporting and analytical tools
	* and, has proven its worth over and over again!

To offer SQL on Hadoop, SQL Query Engines are needed that can query and manipulate large volumes of data stored in HDFS or HBase. Such products are called SQL-on-Hadoop Engines!!

* SQL-on-Hadoop Engines  
	Some of the many SQL-on-Hadoop engines are listed below
	* Apache Drill, 
	* Apache Hive, 
	* CitusDB, 
	* Cloudera Impala, 
	* Concurrent Lingual,
	* Hadapt, 
	* HP Vertica, 
	* InfiniDB, 
	* JethroData, 
	* MemSQL, 
	* Pivotal HAWQ, 
	* Progress DataDirect, 
	* ScleraDB, 
	* Shark,
	* SpliceMachine

* External working of SQL-on-Hadoop Engines
	* On the outside, most of the SQL-on-Hadoop engines look alike. They all support some SQL-dialect that can be invoked through ODBC or JDBC. 
* Internal working of SQL-on-Hadoop Engines
	* Internally, they are very different. The differences stem from the purpose for which they have been designed.
	* 


### 4. Conclusion

### 5. Future Work