MySQL DBA Topologies
====================

These plays are designed to deploy common replication topologies. They are designed for RHEL/CentOS 5, 6, or 7. Currently, the following operations are supported:

Version Installations:
 * Percona Server 5.6
 * Percona Server 5.5
 * MySQL 5.6
 * MySQL 5.5
 * MariaDB 10.0
 * MariaDB 5.5

Topologies:
 * Master/Slave (1 or many slaves)
 * Master/Master

Role Variables
--------------

Servers that will be in a replication topology must have the following parameters assigned to ensure that replication does not break due to conflicts:
 * name
 * server_id
 * parent

MySQL version control is provide through the mysql_version variable. Valid values are mysql_55, mysql_56, ps_55, ps_56, mariadb_55, mariadb_100.

Roadmap
-------

The following functionality is planned but not yet implemented
 * Installing older versions of the available releases
 * Installing to a sandbox instance using dbsake sandbox
 * MySQL MMM
 * MySQL MasterHA
 * Galera

License
-------

BSD

Author Information
------------------

Tyler Mitchell
