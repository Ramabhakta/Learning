# How DB works? Internal Architecture #
## General Components DB ##
1. Network Layer: Take care communication between client and rest of below compoments
2. FrontEnd : Convert query so that remaining componets understand the query (Query in English or any command)
   1. Tokeniser
   2. Parser
   3. Optimiser
3. Query Execution Engine
   1. Query Executor
   2. Cache Managment
   3. Utility : Authentication etc.
4. Manager
   1. Transaction Manager : Also need to review, MVCC (Multi Verion Concurrency Control)
   2. Lock Manager
   3. Recovery Manager
5. Concurreny Manager : Techincally, Lock manager and Concurreny Manager works togther.
6. Storage Engine
   1. Disk Storage Manager
   2. Buffer Manager
   3. Index Manager
7. OS Interaction Layer : Lower level component.
8. For Distributed DB we need below three manager
   1. Shard Manager
   2. Cluster Manager
   3. Replication Manager
  
   
  
   
   
   
      
