This role installs and runs apache kafka in standalone or cluster mode.

Requireаd installed zookeeper.

example playbook:
~~~~
- hosts: kafka
  roles:
    - kafka
~~~~

example inventory:
~~~~
[kafka]
localhost broker_id=0

[zookeeper]
localhost zookeeper_id=0

~~~~
