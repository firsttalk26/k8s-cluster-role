K8s-cluster-role
=========

This role is created for creating kubernetes cluster.

More variables 
----------------
                                                               
During the including role in playbook needed to pass variable  `kubernetes_node`   for setup master node and slave node

variable for Master Node
------------------------


`kubernetes_node: "MasterNode" `

variable for slave node
-----------------------

`kubernetes_node: "SlaveNode" `

Example Playbook
----------------
```
{
     - hosts: all
         tasks: 
           - include_role: 
                name: k8s-cluster-role
             vars: 
               kubernetes_node: "MasterNode"
               
}
```
This playbook will run and configure master node


```
{
     - hosts: all
          tasks: 
            - include_role: 
                 name: k8s-cluster-role
              vars: 
                 kubernetes_node: "SlaveNode"
       

}
```

This playbook will run and configure slave node 

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
