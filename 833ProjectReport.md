# The Development and Application of Hadoop and NoSQL 

## Aarti Parupudi, Quan Kong, Wenbo Wang

### 1. Abstract

### 2. Introduction

#### 2.1 Hadoop

* The reason we need Hadoop
* The functionality of Hadoop
* The implementation and history of Hadoop (Spark) 

#### 2.2 NOSQL

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


### 3. Review of Related Work

#### 3.1 Review on Hadoop

* [MapReduce: Simplified Data Processing on Large Clusters](https://www.usenix.org/legacy/publications/library/proceedings/osdi04/tech/full_papers/dean/dean_html/index.html) (Quan)
* [Understanding the Power of Hadoop as a Service](https://docs.google.com/file/d/0BwMVEMCs7KRNNWIyT3hiRXhLWms/edit) (Aarti)
* [The Hadoop Distributed File System](https://docs.google.com/file/d/0B2_4GOBGjarzTkdLZDBNbVdYTXM/edit) (Quan)


#### 3.2 Review on NoSQL

* [NoSQL Databases](https://docs.google.com/file/d/0B2_4GOBGjarzaTdjcFhoODZVQWs/edit) (Mac)
	* CAP-Theorem
		* **Consistency**: meaning if and how a system is in a consistent state after the execution of an operation. A distributed system is typically considered to be consistent if after an update operation of some writer all readers see his updates in some shared data source.
		* **Availability**: and especially high availability meaning that a system is designed and implemented in a way that allows it to continue operation (i.e. allowing read and write operations) if e.g. nodes in a cluster crash or some hardware or software parts are down due to upgrades.
		* **Partition Tolerance**: understood as the ability of the system to continue operation in the presence of network partitions. These occur if two or more “islands” of network nodes arise which (temporarily or permanently) cannot connect to each other. Some people also understand partition tolerance as the ability of a system to cope with the dynamic addition and removal of nodes.
		* CAP-Theorem - Alternatives, Traits, Examples<p><img src="Content/cap_theorem.png"/></p>
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
* [NoSQL Databases: a step to databases scalability in web environment](https://docs.google.com/file/d/0B2_4GOBGjarzckFhYmxkODNkVUE/edit) (Mac)

#### 3.3 Review on Hadoop + NoSQL

* [Integrating MapReduce and RDBMSs](https://docs.google.com/file/d/0B2_4GOBGjarzS09UbV8tTkR2ems/edit) (Quan)
* [Optimizing Your Enterprise Architecture with Apache Hadoop and NoSQL](https://docs.google.com/file/d/0BwMVEMCs7KRNTjBCSzVQZ0E3OXc/edit) (Aarti)
* [SQL-on-Hadoop Engines Explained](https://docs.google.com/file/d/0BwMVEMCs7KRNb1hici14RV9XVnc/edit) (Aarti)
* [Hadoop and NoSQL Technologies and the Oracle Database](https://docs.google.com/file/d/0BwMVEMCs7KRNUDJwaWx2Y2VyXzA/edit) (Mac)


### 4. Conclusion

### 5. Future Work