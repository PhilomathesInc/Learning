# ReplicationControllers/ReplicaSets

Both have the same purpose but they are not the same  
Replication Controller is the older technology that is being replaced by ReplicaSets  

**Note**
  A key differnce between the two is that ReplicaSets have a mandatory field called selector which specifies the pods that it monitors  
The selector field is not mandatory for replication controller by default it will keep track of the pods defined in the template section

## Scale <br>
Ways to scale the number of pods 

1. Make changes to the number of replicas in yaml file followed by the coomand <br>
`kubectl replace -f replicaset-definiton.yml` <br>

2.  Using the definition file with scale command <br>
  `kubectl scale --replicas=6 -f replicaset-definition.yml` <br>

3. Or provide name in type name format <br>
    `kubectl scale --replicas=6 replicaset myapp-replicaset` 


**Note**  <br>
Using the scale command wont change the number of replicas in the definition file



