# Ansible Playbooks: HDP

A collection of Ansible Playbooks for creating, modifying and administrating HDP

## Prerequisites

* A working environment setup to use the following host groups:

  * hdp: contains all nodes of the cluster
  * utility: the node where the cluster logic and configuration is happening from (Ambari, MySQL, Ranger,...)
  * hadoop: namenodes
  * nimbus: nodes with Storm Nimbus
  * atlas: nodes with Atlas
  * ranger: nodes with Ranger
  * hiveserver: nodes with Hiverserver installed
  * hbase: nodes with HBase Master + HBase Regionserver installed

* The following Ansible roles need to be available (self written, from github.com/condla or from Ansible-Galaxy)
  * hdp-ambari-agents
  * hdp-mysql-server
  * hdp-ambari-server
  * hdp-security
  * hdp-ranger-deploy-certs

* A working environment setup to overwrite the default variables of the roles in use corresponding to the environment
