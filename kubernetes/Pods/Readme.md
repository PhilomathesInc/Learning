# A note about creating pods using kubectl run  

To create a pod from the command line use the command:  

## Create an NGINX pod   
`kubectl run nginx --image=nginx`   
As of version 1.18, kubectl run (without any arguments such as --generator) will create a pod instead of a deployment.  

## To create a deployment using imperative command, use kubectl create:  
`kubectl create deployment nginx --image=nginx` 


## Seeing the list of Pods available <br>
`kubectl get pods`<br>
**To get mode information on pods use:** <br>

`kubectl get pods -o wide`<br>


## To see a verbose description of the pod, use kubectl describe: <br>

`kubectl describe pod 'pod_name'` <br>


## To delete a pod, use kubectl delete <br>
`kubectl delete pod pod_name` <br>


## To make changes to the config of a running pod, use kubectl edit <br>
`kubectl edit -f pod-defintion.yml`<br>
**This doesn't change the content of the definition file** <br>

##  To make changes to the config of a running pod and change the definiton files: <br>
1. Make changes to the definition file <br>
2. `kubectl apply -f pod-definition.yml` <br>
2. 

 
