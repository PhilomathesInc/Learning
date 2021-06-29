# ReplicationControllers/ReplicaSets

Both have the same purpose but they are not the same  
Replication Controller is the older technology that is being replaced by ReplicaSets  

** Note **
  A key differnce between the two is that ReplicaSets have a mandatory fiel called selector which specifies the pods that it monitors  
The selector field is not mandatory for replication controller by defaultit will keep track of the pods with labels which is defined in the definition section
