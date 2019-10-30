This role installs and runs apache zookeeper in standalone or cluster mode.

example playbook:
~~~~
- hosts: zookeeper
  roles:
    - zookeeper
~~~~

example inventory:
~~~~
[zookeeper]
host1 zookeeper_id=0
...
host_N zookeeper_id=N
~~~~
