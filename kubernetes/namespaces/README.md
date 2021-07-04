Three namespaces created automatically:

1. Default: This is where a User works by default.
2. kube-system: Pods and services created for internal purpose
   are created in this namespace eg. Those those required by its networking
   solutions the dns service to isolate these from the user and prevent user from 
   accidentally modifying these services.
3. kube-public: This is where resources that should be made available to all the users are created.

Resources within a namespace can refer to each other simply by using their names    
