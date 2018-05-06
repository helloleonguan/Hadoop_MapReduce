## Lesson 02 - HDFS & MapReduce 

### 1. HDFS Data Storage
* data files are often split into big chunks in __HDFS__ (e.g. 64Mb per block) and they are named as blk_i where i is a large number. 
* Each chunk is then stored into one of the nodes in the cluster. 
* Meta-data is stored on the NameNode so that we can know which blocks on diff nodes compose of the original file. 
* Issues that __HDFS__ faces: disk failure on DataNode or NameNode, network failure in the cluster. 
* Data Redundancy: each block is replicated 3 times and stored on diff DataNodes to avoid the DataNode failure. 
* Info on NameNode is also stored on Network File System (a.k.a. NFS) & another standby NameNode to avoid NameNode failure or network failure on NameNode. 

### 2. HDFS Commands
It starts with "hadoop fs -" and then following by normal unix system commands. 

### 3. MapReduce Data Processing 
* Multiple blocks are processed in parallel. 
* Mappers: work on a small fraction of the original data and produce _intermediate records_ which are key-value pairs.
* Shuffle & Sort: move _intermediate records_ to Reducers + sort them. 
* Reducers: work on 1 set of records at a time from (key, values) sets and produce the final result. 

