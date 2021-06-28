# A not about creating pods using kubectl run  

To create a pod from the command line use the command:  

## Create an NGINX pod   
`kubectl run nginx --image=nginx`   
As of version 1.18, kubectl run (without any arguments such as --generator) will create a pod instead of a deployment.  

## To create a deployment using imperative command, use kubectl create:  
`kubectl create deployment nginx --image=nginx`  