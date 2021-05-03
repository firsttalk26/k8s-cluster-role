K8s-cluster-role
=========

This role is created for creating kubernetes cluster.

More variables 
----------------
                                                               
During the including role in playbook needed to pass variable  `kubernetes_node`   for setup master node and slave node

variable for Master Node
------------------------


`kubernetes_role: "MasterNode" `

variable for slave node
-----------------------

`kubernetes_role: "SlaveNode" `

Example Playbook
----------------
```
{

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }
}
```
License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
