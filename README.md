# How DB works? Internal Architecture #
##Client Components##
1. Network Layer
2. FrontEnd
   1. Tokeniser
   2. Parser
   3. Optimiser
3. Query Execution Engine
   1. Query Executor
   2. Cache Managment
   3. Utility : Authentication etc.
4. Manager
   1. Transaction Manager
   2. Lock Manager
   3. Recovery Manager
5. Concurreny Manager : Techincally, Lock manager and Concurreny Manager works togther.
6. Storage Engine
   1. Disk Storage Manager
   2. Buffer Manager
   3. Index Manager
7. OS Interaction Layer : Lower level component.
   
   
      
