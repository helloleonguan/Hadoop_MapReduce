## Lesson 01 - Big Data 

### 1. Definition of Big Data 

Big Data is a loosely defined term used to describe data sets so large and complex that they become awkward to work with using standard statistical software. (International Journal of Internet Science, 2012, 7 (1), 1–5)

### 2. Challenges of Big Data 

* Data is created very fast.
* Data comes from various sources. 
* Data comes in with various formats. 

### 3. [3Vs Data Management](https://blogs.gartner.com/doug-laney/files/2012/01/ad949-3D-Data-Management-Controlling-Data-Volume-Velocity-and-Variety.pdf)

* Volumns: size of data
  * cheaper way of storing data reliably
  * also relates to stream through networks and read/process data
  * __Hadoop__ stores massive data in a distributed way across multiple machines. 
* Variety: diff sources + diff formats
  * Relational Databases: SQL Server, MySQL
  * Data Warehouses from Oracle and IBM
  * Unstructured & Semi-structured data 
  * __Hadoop__ accepts all formats of data 
* Velocity: speed of data arrived & the speed of processing data
  * avoid discarding data 
  * more data == more useful/insightful info 

### 4. [The Google File System](http://static.googleusercontent.com/media/research.google.com/en/us/archive/gfs-sosp2003.pdf)  

### 5. [Google's Processing Framework - _MapReduce_](http://static.googleusercontent.com/media/research.google.com/en/us/archive/mapreduce-osdi04.pdf)  

### 6. HDFS 
- Hadoop Distributed File System to store data. Usually a cluster of machines. 
- MapReduce to Process Data. 

### 7. Hadoop Ecosystem
- e.g. _Hive_ (write SQL-ish statments for long batch processing), _PIG_ (simple scripting language): both of them translated into __MapReduce__ to access __HDFS__. 
- e.g. _Imapala_ (SQL-ish statements) directly interacts with __HDFS__ with low latency.
- e.g. _Sqoop_, _Flume_: take traditional relational databases into __HDFS__.
- e.g. HBase: real-time database which is built on __HDFS__. 
- e.g. _Hue_: GUI for the __HDFS__ cluster. 
- e.g. _Oozie_: workflow management tool. 
- e.g. _Mahout_: a ML library. 
- __CDH__: a complete system for all of the above. 

