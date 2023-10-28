Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

| Name                                   | Description                                             | Default
|----------------------------------------|---------------------------------------------------------|------------------------------------------------
| clickhouse_keeper_server_port          | Port number to be used by clients of keeper             | 9181 default equivalent of 2181 as in zookeeper
| clickhouse_keeper_peer_port            | Port number to listen to interserver keeper connections | 9444
| clickhouse_keeper_server_id            | Identifier of the keeper server for raft configuration  | compute from the name of the server
| clickhouse_keeper_operation_timeout_ms | Time for operations to expire in milliseconds           | 10000
| clickhouse_keeper_session_timeout_ms   | Time for sessions to expire in milliseconds             | 30000
| clickhouse_keeper_raft_logs_level      | Level of the logs for the raft protocol                 | info

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
