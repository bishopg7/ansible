This role creates docker swarm cluster and installs portainer agents on it.  
The case was to install cluster on VM`s without internet.
It uses private docker registry and proxy for yum and pip located in private nexus.


example playbook:
~~~~
- hosts: docker_swarm_cluster
  roles:
    - docker_swarm_cluster
~~~~

example inventory:
~~~~
[swarm_manager]
host1
host2
host3

[swarm_worker]
host4
host5
host6

[docker_swarm_cluster:children]
swarm_manager
swarm_worker

~~~~
